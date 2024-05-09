# Lab Report 3

By Sammy Hamouda

## Part 1 - Bugs

### 1. Failure-inducing code

```
@Test
public void testAverageWithoutLowest(){
  double[] input = {3.400, 5.50, 2.10, 2.100};
  assertEquals(4.45, ArrayExamples.averageWithoutLowest(input), 0.1);
} 
```

### 2. Working code

```
@Test
public void testAverageWithoutLowestEmpty(){
  double[] input = {};
  assertEquals(0.0, ArrayExamples.averageWithoutLowest(input), 0.1);
}
```


### 3. Symptom output
![TestOutput.png](/images/LB3/TestOutput.png)



### 4. The bug before and after

#### Before
```
static double averageWithoutLowest(double[] arr) {
  if(arr.length < 2) { return 0.0; }
  double lowest = arr[0];
  for(double num: arr) {
    if(num < lowest) { lowest = num; }
  }
  double sum = 0;
  for(double num: arr) {
    if(num != lowest) { sum += num; }
  }
  return sum / (arr.length - 1);
}
```

#### After
```
static double averageWithoutLowest(double[] arr) {
  if(arr.length < 2) { return 0.0; }
  double lowest = arr[0];
  int count = 0;
  for(double num: arr) {
    if(num < lowest) { lowest = num; }
  }
  double sum = 0;
  for(double num: arr) {
    if(num != lowest) { 
      sum += num; 
    }else{
      count++;
    }
  }
  return sum / (arr.length - count);
}
```

### How the fix works
The original bug was the fact that averageWithoutLowest didn't account for the fact that there could be duplicates of the lowest number. This led to the average without being incorrectly calcuated. My fix addresses this by adding a counter that counts how many times the lowest number appears in the array, and then subtracting the array length by that count instead of just 1, which doesn't account for the fact that multiple numbers are possibly taken out of the lowest number appears multiple times.

## Part 2 - Researching Commands


### less with 

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

### less with 

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

### less with 

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

### less with 

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful

```
samham@penguin:~/$ ls lecture1
Hello.class Hello.java messages README workspace.code-workspace
```
Sentence describing why this is useful
