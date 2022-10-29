#Python #Programming 
# How it's done
- Main idea: *Make the I/O function/library a parameter*. Now you can plug in any other I/O library function.
```python
def fun(url, requests=requests):
	response = requests.get('url')

# now you can plug(inject) in any request library you want:
fun('google.com', requests)
fun('google.com', httpx)
fun('google.com', urllib3)
...
```
* Testing is done via *simulating one of the dependencies*:
```python
class FakeRequests:
	def get(self, url):
		return 'whatever'
```
This is what a test would look like for the `fun` function defined above
```python
def test_fun():
	fake = FakeRequests()
	# we use the fake library to create a fake request, 
	# the same way we would with a real library
	faked_fun = fun('google.com', fake)
	
	# now we don't actually have to spend time
	# waiting for the request, and we can 
	# run the test offline too! pretty cool
	assert fake.get(), 'something'
```
# Problems
1. The `FakeRequests` is not actually a requests library. The fact that we call it and get data back doesn't mean that it's going to be the same for a real library (maybe the `.get()` doesn't return data for every library. Maybe there is no `.get()` function in some library)
2. Simple for small things, but a pain to implement for bigger systems

