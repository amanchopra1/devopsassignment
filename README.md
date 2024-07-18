# DevOps Assignment

This repository contains two assignments focused on utilizing Jenkins and Docker to automate testing and deployment processes for different types of applications.

## Assignments

### 1. Automated Testing with Jenkins and Docker

**Objective:** Utilize Jenkins to automate the testing process of a Python Django-based web application within a Docker container.

#### Steps:
1. **Develop a Web Application:**
   - Create a Python Django web application.
   - Write test cases using a testing framework like `pytest`.

2. **Create a Dockerfile:**
   - Include the application and the necessary testing tools in the Dockerfile.

3. **Set Up a Jenkins Pipeline:**
   - **Pull the source code.**
   - **Build the Docker image.**
   - **Run the tests inside the Docker container.**
   - **Report the test results.**

### 2. Maven Project with Docker and Jenkins

**Objective:** Use Jenkins to automate the build, test, and deployment of a Maven-based Java application in a Docker container.

#### Steps:
1. **Develop a Simple Maven-Based Java Application:**
   - Create a basic Java application using Maven.

2. **Create a Dockerfile:**
   - Include the application and the necessary testing tools in the Dockerfile.

3. **Set Up a Jenkins Pipeline:**
   - **Pull the source code.**
   - **Build the Docker image.**
   - **Run the tests inside the Docker container.**
   - **Report the test results.**

## Installation and Usage

### 1. Automated Testing with Jenkins and Docker

#### Clone the Repository:
```sh
git clone https://github.com/amanchopra1/devopsassignment.git
cd devopsassignment/python-django-app

docker build -t django-app .
docker run -p 8000:8000 django-app

docker run django-app pytest

git clone https://github.com/amanchopra1/devopsassignment.git
cd devopsassignment/java-maven-app


docker build -t maven-app .
docker run maven-app

Using Jenkins Pipelines

Jenkins Pipeline for Python Django Application:

	•	Pull the source code from the repository.
	•	Build the Docker image using the Dockerfile.
	•	Run the Docker container and execute the tests.
	•	Publish the test results.

Jenkins Pipeline for Maven Java Application:

	•	Pull the source code from the repository.
	•	Build the Docker image using the Dockerfile.
	•	Run the Docker container and execute the tests.
	•	Publish the test results.

Test Cases:
import pytest
from django.test import TestCase

class MyTests(TestCase):
    def test_example(self):
        self.assertEqual(1 + 1, 2)

Maven Java Application:
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;

public class MyJavaTests {

    @Test
    public void testExample() {
        assertEquals(2, 1 + 1);
    }
}



