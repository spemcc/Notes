``c++
	template< size_t N>
	void check_bounds_compile_time(int (&ar1)[N], int (&ar2)[N])
	{
  
  		...
	}

	int ar[10];
	int ar2[10];
	check_bounds(ar, ar2); // GOOD
  
	int arr[20];
	int arr2[10];
	check_bounds(arr, arr2); //BAD - Wont compile
```
