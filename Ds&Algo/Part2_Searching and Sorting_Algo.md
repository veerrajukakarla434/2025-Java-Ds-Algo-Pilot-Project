# Searching and Sorting

* #### Linear Search
* #### Binary Search


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



