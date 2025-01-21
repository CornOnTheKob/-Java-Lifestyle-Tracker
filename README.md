# Lifestyle Tracker JAVA GUI

Description: This project was developed as part of my Introduction to Programming I course, allowing users to monitor their lifestyle habits.

## How to Run [in Terminal]

1. [Clone](https://docs.github.com/en/repositories/creating-and-managing-repositories/cloning-a-repository) this repository into your working machine.
2. Make sure that you have [Java](https://www.oracle.com/java/technologies/downloads/) installed on your machine. It is recommended to use Java 8 or older.
3. Run the command line. Change your working directory to the directory where you cloned this repository. A bunch of `.java` files can be found there. Check by typing `dir` on Windows or `ls` on macOS/Linux in your command line. Once there, enter the following commands:

    ```console
    $ javac *.java
    $ java TrackerApp.java
    ```

## How to Use

In this JFrame, the GUI is segregated into at least 3 JPanels:

### Panel 1
- User will input his/her name to enable all the JButtons.  
- User can now utilize the JButtons as well as use JOptionPanes to record:
  - Food and its calories  
  - Food eaten and its servings  
  - Total calories consumed  
  - (Same applies to activities).  
- User can also print the Report and Mystery Report, as well as activate Mystery Mode through one of the given buttons.

### Panel 2
- Using JTables, the user can view the following:
  - List of Food  
  - List of Food Eaten  
  - List of Activities  
  - List of Activities Performed  
- The programmer used various classes such as Default Table Model, JTables, and other utilities from the Java catalogue.  
- The user can also switch views using JButtons. Two of the buttons allow the user to edit:
  - **List of FOOD ATE**:
    - Edit the name and servings (for food).  
  - **List of ACTIVITIES PERFORMED**:
    - Edit the name and hours performed (for activities).  
- If the user inputs a new name not found within the list of Foods Recorded / Activities Performed, the program will:
  - Ask for the calories that activity consumes/burns (per serving or per hour).  
- If the name is found:
  - Only ask for the servings/hours performed.

### Panel 3
- Using JTextArea, the program will print out one of the following:
  - **1)** A prompt welcoming the user to the lifestyle tracker.  
  - **2)** `Report()` - prints a "receipt" that includes:  
    - List of food consumed  
    - Total calories consumed  
    - List of activities performed  
    - Total calories burned  
    - Net calories for the day  
    - Forecast of weight gain/loss after a week, a month, 3 months, and 6 months.  
  - **3)** Mystery Mode - an add-on that takes new inputs from the user, such as:  
    - Gender  
    - Age  
    - Height  
    - Weight  
    - Weight goal type  
    - Target weight  
    - Time period  
    - Activity level  

From these inputs, it calculates the following:
- **BMI**: Indicates the category of your weight.  
- **BMR (Basal Metabolic Rate)**: Calculates the calories needed for basic life-sustaining functions.  
- **Calories to sustain weight**: Calories needed per day to maintain your weight.  
- **Calories to target weight**: Calories needed per day to reach your target weight.  
- **Calories to gain/lose weight**: How many calories you need to consume more or less per day.  

Integrating the new inputs with the old inputs:  
- The **Activity Level** will cross-check the list of activities performed and make research-based assumptions depending on the duration of activities.  
- Based on recorded daily food intake, it provides guidance on how many calories to consume or burn, depending on the inputs.

- A **Clear Report** button is available at the lower part of the JPanel to clear the text area.

---

Have Fun! - Kobi
