## Data Structures & Algorithms 

#### Learning Outcomes

* Algorithms and Metrics : Time and Space Complexcity analysis
* Data Structures : Linked Lists, Queues, Stacks, Heap, Tree, Dictionary
* Recursion Algorithms
* Sorting Algorithms : Bubble sort, Comb Sort, Selection sort, Merge Sort, Quick sort
* Graphs : Data Structures Of Graphs, BFS, DFS
* String Releated Algorithms
* Divid and Conquer Algorithms

## Algorithms 

![alg](https://github.com/veerrajukakarla434/VRK-DataStructures-Algorithms/blob/master/alg.JPG "alg")

![image](https://user-images.githubusercontent.com/40323661/161489250-eabce4a0-ac23-4b93-b68c-88d34c25efaa.png)

## Analysis of Algorithms | Set 1 (Asymptotic Analysis)

#### Why performance analysis?

* There are many important things that should be taken care of, like user friendliness, modularity, security, maintainability, etc. 
* **Why to worry about performance?**
* The answer to this is simple, we can have all the above things only if we have performance. So performance is like currency through which we can buy all the above things. Another reason for studying performance is – speed is fun!
To summarize, performance == scale. Imagine a text editor that can load 1000 pages, but can spell check 1 page per minute OR an image editor that takes 1 hour to rotate your image 90 degrees left OR … you get it. If a software feature can not cope with the scale of tasks users need to perform – it is as good as dead.

#### Given two algorithms for a task, how do we find out which one is better?

* One naive way of doing this is – implement both the algorithms and run the two programs on your computer for different inputs and see which one takes less time. There are many problems with this approach for analysis of algorithms.
* 1) It might be possible that for some inputs, first algorithm performs better than the second. And for some inputs second performs better.
* 2) It might also be possible that for some inputs, first algorithm perform better on one machine and the second works better on other machine for some other inputs.

#### Asymptotic Analysis

* **Asymptotic Analysis** is the big idea that handles above issues in analyzing algorithms. 
* In Asymptotic Analysis, we evaluate the performance of an algorithm in terms of input size (we don’t measure the actual running time). We calculate, how the time (or space) taken by an algorithm increases with the input size.

![image](https://user-images.githubusercontent.com/40323661/161790455-f7749d31-a6f7-4236-990f-ae99c0dbd786.png)

![image](https://user-images.githubusercontent.com/40323661/161790630-11a7e7a3-78f5-461f-99fa-2ccd4a9c74e2.png)

![image](https://user-images.githubusercontent.com/40323661/161790998-94531343-8487-403c-8c84-82eb16790a56.png)

* Set1 Video Reference : https://www.youtube.com/watch?v=QJMtPlYPQTA

## Analysis of Algorithms | Set 2 (Worst, Average and Best Cases)

![image](https://user-images.githubusercontent.com/40323661/161792575-e058b7b8-fb33-48d1-80c1-0c8ece53307d.png)

```Java
// Java implementation of the approach
 
public class GFG {
 
    // Linearly search x in arr[].  If x is present then
    // return the index, otherwise return -1
    static int search(int arr[], int n, int x)
    {
        int i;
        for (i = 0; i < n; i++) {
            if (arr[i] == x) {
                return i;
            }
        }
        return -1;
    }
 
    /* Driver program to test above functions*/
    public static void main(String[] args)
    {
        int arr[] = { 1, 10, 30, 15 };
        int x = 30;
        int n = arr.length;
        System.out.printf("%d is present at index %d", x,
                          search(arr, n, x));
    }
}
 
 ```
 ![image](https://user-images.githubusercontent.com/40323661/161795299-e087b7f8-a267-487a-a7bf-04052c9eabe5.png)

![image](https://user-images.githubusercontent.com/40323661/161795521-0e540dbb-328a-4457-b603-02dd3cce6284.png)

![image](https://user-images.githubusercontent.com/40323661/161796454-79ea6590-ea55-4a33-a688-030ec29f10e2.png)

![image](https://user-images.githubusercontent.com/40323661/161796577-f8e3d195-d689-41e2-9cd4-aec2c834cec2.png)

![image](https://user-images.githubusercontent.com/40323661/161796632-d76f31e1-7bb2-4ad3-bc5e-3cd7f2a7474c.png)

![image](https://user-images.githubusercontent.com/40323661/161797104-5f6ea784-13b6-4d78-a3c1-037019830b95.png)

## Analysis of Algorithms | Set 3 (Asymptotic Notations)

![image](https://user-images.githubusercontent.com/40323661/161797519-ef935f7d-81e5-47f8-b11f-dc229afe7787.png)

![image](https://user-images.githubusercontent.com/40323661/161799555-9eea7703-6346-4f9f-aff8-460a68583665.png)

![image](https://user-images.githubusercontent.com/40323661/161800060-574d3c32-a205-4bd5-a05f-1e89ef67d2d1.png)

![image](https://user-images.githubusercontent.com/40323661/161800243-59ba5943-8f37-4fa8-88c4-7c8844fac2d8.png)

* Reference Link : https://www.geeksforgeeks.org/analysis-of-algorithms-set-3asymptotic-notations/

## Analysis of Algorithms | Set 4, (Analysis of Loops)  Set 4 (Solving Recurrences),  Set 5 (Amortized Analysis Introduction)

* RefLink : https://www.geeksforgeeks.org/analysis-of-algorithms-set-4-analysis-of-loops/
* https://www.geeksforgeeks.org/analysis-algorithm-set-5-amortized-analysis-introduction/?ref=lbp

## What does ‘Space Complexity’ mean?

![image](https://user-images.githubusercontent.com/40323661/161801162-514b22b7-434e-4687-acd8-1dbe8300e0a5.png)

* Ref: link https://www.geeksforgeeks.org/g-fact-86/?ref=lbp










