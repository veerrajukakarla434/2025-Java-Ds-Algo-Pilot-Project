# Searching and Sorting

* **Linear Search**
* **Binary Search**
* **Selection Sort**


## Linear Search

![image](https://user-images.githubusercontent.com/40323661/161802901-71b03da0-4c61-425e-bb1f-1fb5aba81351.png)

![image](https://user-images.githubusercontent.com/40323661/161803044-6c18116a-4e2b-4d81-9797-0b51fd2be2c8.png)

![image](https://user-images.githubusercontent.com/40323661/161803175-ec500670-b204-4776-9ba9-60eb786baddf.png)

* Ref Link : https://www.geeksforgeeks.org/linear-search/

```Java
// Java code for linearly searching x in arr[]. If x
// is present then return its location, otherwise
// return -1

class GFG
{
	public static int search(int arr[], int x)
	{
		int n = arr.length;
		for (int i = 0; i < n; i++)
		{
			if (arr[i] == x)
				return i;
		}
		return -1;
	}

	// Driver code
	public static void main(String args[])
	{
		int arr[] = { 2, 3, 4, 10, 40 };
		int x = 10;

		// Function call
		int result = search(arr, x);
		if (result == -1)
			System.out.print(
				"Element is not present in array");
		else
			System.out.print("Element is present at index "
							+ result);
	}
}

```
![image](https://user-images.githubusercontent.com/40323661/161803675-4b8bd3b5-b4c8-4b1d-8a0e-0d270ddf98ae.png)

## Binary Search
![image](https://user-images.githubusercontent.com/40323661/161907952-8e9ac669-c619-49f8-b662-3542ba0ed4b1.png)

![image](https://user-images.githubusercontent.com/40323661/161907999-339759da-0c9e-4645-a0f8-d36be245a48f.png)

![image](https://user-images.githubusercontent.com/40323661/161908647-6d24ecec-f18d-4784-bf19-c5c2d7d7b600.png)

![image](https://user-images.githubusercontent.com/40323661/161908780-72f83e81-270f-4f83-ac8f-8ae38e277ae7.png)

![image](https://user-images.githubusercontent.com/40323661/161909071-cb86dfe7-02c6-451e-bc43-6aa5fd31fbe1.png)

#### Example
```java
// Java implementation of recursive Binary Search
class BinarySearch {
	// Returns index of x if it is present in arr[l..
	// r], else return -1
	int binarySearch(int arr[], int l, int r, int x)
	{
		if (r >= l) {
			int mid = l + (r - l) / 2;

			// If the element is present at the
			// middle itself
			if (arr[mid] == x)
				return mid;

			// If element is smaller than mid, then
			// it can only be present in left subarray
			if (arr[mid] > x)
				return binarySearch(arr, l, mid - 1, x);

			// Else the element can only be present
			// in right subarray
			return binarySearch(arr, mid + 1, r, x);
		}

		// We reach here when element is not present
		// in array
		return -1;
	}

	// Driver method to test above
	public static void main(String args[])
	{
		BinarySearch ob = new BinarySearch();
		int arr[] = { 2, 3, 4, 10, 40 };
		int n = arr.length;
		int x = 10;
		int result = ob.binarySearch(arr, 0, n - 1, x);
		if (result == -1)
			System.out.println("Element not present");
		else
			System.out.println("Element found at index "
							+ result);
	}
}
```

```Java
package com.algo;

public class BinarySearch1 {

	public static void main(String[] args) {
		
		int arr[] = {10,30,40,50,60,70,80,90};
		int l=0;
		int r = arr.length;
		int x = 60;
		
		int result = binarySearch(arr,l,r,x);
		
		if(result==-1) {
			System.out.println("Element is not present given arry "+ result);
		}else {
			
			System.out.println(x +" Element is present given arry index "+ result);
		}
      
	}
	
	
	static int binarySearch(int arr[], int l, int r, int x) {
		
		 if(r>=l) {
			 int mid = l+(r-l)/2;
			 
			 if (arr[mid]==x) {
				 return mid;
			 }
			 
			 if(arr[mid] > x) {
				 
				return binarySearch(arr,l, mid-1, x);
			 }
			 
			 if(arr[mid] < x) {
				 
					return binarySearch(arr,mid+1, r, x);
				 }
		 }
		
		return -1;
	}

}
```

* If Array is unsorted for binary search we can use one of the sorting algo or arrays.sort() method.

## Selection Sort

![image](https://user-images.githubusercontent.com/40323661/162649392-1687a9f9-d113-4fcf-ab56-887880fc1961.png)

![image](https://user-images.githubusercontent.com/40323661/162649430-b51e09fa-f684-40db-bd63-e9405917cf5d.png)





