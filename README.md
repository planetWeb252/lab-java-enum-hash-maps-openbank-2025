![logo_ironhack_blue 7](https://user-images.githubusercontent.com/23629340/40541063-a07a0a8a-601a-11e8-91b5-2f13e4e6b441.png)

# LAB Java | Enums & HashMaps

## Introduction

We have just learned how to use Enums and HashMaps so let's practice a bit more.

<br>

## Requirements

1. Fork this repo.
2. Clone this repo.
3. Add your instructor and the class graders as collaborators to your repository. If you are unsure who your class graders are, ask your instructor or refer to the day 1 slide deck.
4. In the repository, create a Java project and add the code for the following prompts.

## Submission

Once you finish the assignment, submit a URL link to your repository or your pull request in the field below.

<br>

## Instructions

1. Create a new Java project in your preferred development environment.
2. In the project, create a class called `Student` that contains the following properties:
   - `name`: String
   - `grade`: int (in the range 0-100)
3. Create a `Map` with a key of the student's name (String) and a value of a `Student` object.
4. Create a method called `increaseGrades` that takes a `Map<String, Student>` as a parameter, increases every student's grade by 10% and returns the updated map.
5. Create 4 Student objects for your classmates and add them to the `Map`.

<br>

## FAQs

<br>

<details>
  <summary style="font-size: 16px; cursor: pointer; outline: none; font-weight: bold;">I am stuck and don't know how to solve the problem or where to start. What should I do?</summary>

<br> <!-- ✅ -->

If you are stuck in your code and don't know how to solve the problem or where to start, you should take a step back and try to form a clear, straight forward question about the specific issue you are facing. The process you will go through while trying to define this question, will help you narrow down the problem and come up with potential solutions.

For example, are you facing a problem because you don't understand the concept or are you receiving an error message that you don't know how to fix? It is usually helpful to try to state the problem as clearly as possible, including any error messages you are receiving. This can help you communicate the issue to others and potentially get help from classmates or online resources.

Once you have a clear understanding of the problem, you should be able to start working toward the solution.

  <br>

</details>

<br>

<details>
  <summary style="font-size: 16px; cursor: pointer; outline: none; font-weight: bold;">How do I create a Maven project in IntelliJ?</summary>

<br> <!-- ✅ -->

To create a Maven project in IntelliJ, you can follow these steps:

1. Open IntelliJ IDEA and click the "Create New Project" button.
2. In the "New Project" dialog, select "Maven" as the build system.
3. Specify the name of the project.
4. In the "Project Location" section, specify a location where you want to save your project.
5. Select the "Create Git repository" checkbox in order to initialize the git repository upon creation of the project.
6. Click the "Create" button to create the Maven project.

  <br>

</details>

<br>

<details>
  <summary style="font-size: 16px; cursor: pointer; outline: none; font-weight: bold;">How do I use "HashMaps" in Java and how can I print them?</summary>

<br> <!-- ✅ -->

A `HashMap` in Java is a data structure that stores key-value pairs. It is implemented as an unordered map, meaning that the order of the elements may change over time.

Here's an example of how you can create and use a `HashMap` in Java:

```java
import java.util.HashMap;

public class Main {
    public static void main(String[] args) {
        HashMap<String, Integer> map = new HashMap<>();
        map.put("Key 1", 1);
        map.put("Key 2", 2);
        map.put("Key 3", 3);

        System.out.println("Value of Key 1: " + map.get("Key 1"));
        System.out.println("Value of Key 2: " + map.get("Key 2"));
        System.out.println("Value of Key 3: " + map.get("Key 3"));
    }
}
```

In the example above, we first create a `HashMap` map that stores String keys and Integer values. We then use the `put` method to add three key-value pairs to the map. Finally, we use the `get` method to retrieve and print the values associated with each key.

To print the entire `HashMap`, you can use a `forEach` loop:

```java
map.forEach((key, value) -> System.out.println("Key: " + key + ", Value: " + value));
```

In this example, the `forEach` loop iterates over each key-value pair in the `HashMap` and prints the key and value.

  <br>

</details>

<br>

<details>
  <summary style="font-size: 16px; cursor: pointer; outline: none; font-weight: bold;">I am unable to push changes to my repository. What should I do?</summary>

<br> <!-- ✅ -->

If you are unable to push changes to your repository, here are a few steps that you can follow:

1. Check your internet connection: Ensure that your internet connection is stable and working.
1. Verify your repository URL: Make sure that you are using the correct repository URL to push your changes.
1. Check Git credentials: Ensure that your Git credentials are up-to-date and correct. You can check your credentials using the following command:

```bash
git config --list
```

4. Update your local repository: Before pushing changes, make sure that your local repository is up-to-date with the remote repository. You can update your local repository using the following command:

```bash
git fetch origin
```

5. Check for conflicts: If there are any conflicts between your local repository and the remote repository, resolve them before pushing changes.
6. Push changes: Once you have resolved any conflicts and updated your local repository, you can try pushing changes again using the following command:

```bash
git push origin <branch_name>
```

</details>
