# Mocking

#Python #Programming

- Main idea - you replace parts that are long to compute, (or require internet)
- Allows you to simulate different behaviours (temporarily replace the return value, implement some side effect).

```python
def test_fun():
	fake = FakeRequests()
	faked_fun = requests.get('google.com', fake)

	# replace the requests.get in fun with our fake
	with patch('requests.get', fake.get()):
		faked_fun = fun('google.com')
	assert fake.get(), 'something'
```
