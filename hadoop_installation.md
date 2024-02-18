# Hadoop Installation for Windows

Hadoop is a powerful framework for distributed storage and processing of large data sets. In this guide, we will walk through the step-by-step process of installing Hadoop on a Windows environment, ensuring a smooth setup for running Hadoop programs.

## Step 1: Download Hadoop

Begin by downloading the latest version of Hadoop from the official Apache Hadoop releases page: [https://hadoop.apache.org/releases.html](https://hadoop.apache.org/releases.html).

## Step 2: Download and Install WinRaR

Ensure you have WinRaR installed on your system, as it will be used to extract the downloaded Hadoop files.

## Step 3: Extract Hadoop Files

Open the downloaded Hadoop zip file using WinRaR and extract the contents to the C drive.

## Step 4: Download and Configure JDK

Download the Java Development Kit (JDK) and copy it into the "java" folder in the C drive. Set the JAVA_HOME in the path variables to "C:\Java\jdk1.8.0_281\bin". Edit the system variable path and add the new path.

## Step 5: Configure Hadoop

Navigate to the Hadoop folder extracted in step 3. Inside the "etc" directory, edit the "hadoop-env" file and set JAVA_HOME to "C:\Java\jdk1.8.0_281". Add an HADOOP_HOME variable with the path "C:\hadoop\bin".

## Step 6: Verify Installation

Open a command prompt and type the commands `hadoop` and `hadoop -version` to ensure the installation is successful.

## Hadoop Program Run Instructions

1. Open the command prompt in the directory containing the Hadoop project.
2. Run the Hadoop program file using the command: 
   ```bash
   hadoop jar trip.jar inputpath output


# Downloading JAR File for Hadoop Program

To create a JAR file for your Hadoop program, follow these steps:

1. Right-click on the project.
2. Select "Export."
3. Choose "JAR file" from the options.
4. Select the project and classes needed for your Hadoop program.
5. Save the JAR file in the project folder.

# Troubleshooting Hadoop Errors

If you encounter errors while running Hadoop projects on Windows, follow these steps to troubleshoot:

1. Windows may throw errors due to a lack of support for binary formats. Download `winutils` and `hadoop.dll` from GitHub, ensuring that the versions match your installed Hadoop version.

By diligently following these comprehensive steps, you are now well-equipped to harness the power of Hadoop on your Windows system. Happy coding!
