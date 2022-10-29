#Python #Programming 
- Main idea - you simulate certain behaviors of already existing functions, in order to test specific behaviors of specific parts of the program.

# Python `mock`
- Allows you to simulate different behaviours (temporarily replace the return value, implement some side effect). 
```python
def test_fun():
	fake = FakeRequests()
	faked_fun = fun('google.com', fake)

	# replace the requests.get in fun with our fake
	with patch('requests.get', fake.get()):
		faked_fun = fun('google.com')
	assert fake.get(), 'something'
```