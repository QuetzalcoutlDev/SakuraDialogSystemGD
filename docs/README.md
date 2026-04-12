# Getting Started Guide 💡

This guide is designed to help you quickly understand the concepts of Sakura Dialog System.

## Requirements

- Install the latest version of GDevelop
- Install the latest version of Visual Studio Code
- Download the Sakura Script extension from [here](https://github.com/QuetzalcoutlDev/sakura-script/releases/).
- Download and install the Sakura Dialog System extension in your project [download it here](https://github.com/QuetzalcoutlDev/SakuraDialogSystemGD/releases/)

# Conditions, actions and expressions

Once you meet all the requirements, we can begin explaining the conditions and actions.

If you haven't installed the extension, simply open the GDevelop sidebar menu and click the + button in the "Extensions" section.

![how_to_install](/img/for_docs/how_to_install.png)

Click on "import extension" and locate the Sakura Dialog System extension you downloaded.

If you installed the extension correctly, you should see "Sakura Dialog System" listed in the conditions and actions menu.

![conditions](/img/for_docs/in_conditions.png) 
![actions](/img/for_docs/in_actions.png)

## Conditions

Conditions are like internal questions that GDevelop asks the extension to see if what you are asking is true, therefore, do something, and if it is false, also do something (if you want).

### Dialog is running
![running](/img/for_docs/condition_0.png)

Verify that the dialog is running.

### Get line type
![line](/img/for_docs/condition_1.png)

It retrieves the current line type, which can be: "dialogue", "options", "command", or "conditionals".

You can then trigger an action if one of these lines is present.

### Command called
![called](/img/for_docs/condition_2.png)

It retrieves the name of the custom command and allows you to obtain its parameters.

## Actions

Actions are events that must be performed if a condition is met or that must always be performed.

### Load dialog file
![load_dialog](/img/for_docs/action_0.png)

Loads a dialog file in .json format, exported from Visual Studio Code.

All actions, conditions, and expressions will be executable once this action is used.

![load_file_example](/img/for_docs/load_file_example.png)

> [!NOTE]
> Avoid clicking "Create/Edit with Yarn" at all costs, as this will cause the dialog system to fail. Yarn is not compatible with the Sakura Script dialog format, and vice versa.

### Go to branch
![go_to_branch](/img/for_docs/action_1.png)

Go to a new dialog branch within your loaded dialog file.

### Go to next line
![next_line](/img/for_docs/action_2.png)

Advance to the next line of dialogue.

### Confirm option selection
![confirm_option](/img/for_docs/action_3.png)

Confirm your selection using its index.

> [!NOTE]
> If you have 4 options, the first option has an index of 0, the second 1, and so on.

### Stop dialogue
![stop_dialogue](/img/for_docs/action_4.png)

Stop the execution of the dialogue.

### Save State
![save_state](/img/for_docs/action_5.png)

Save the dialog state in a variable.

> [!NOTE]
> This does not save your characters' positions (you'll need to do that manually) or previously saved commands.

### Load State
![load_state](/img/for_docs/action_6.png)

Load the dialog state from a variable.

> [!NOTE]
> This action currently does not take into account changes to the dialog file (e.g., you changed or deleted a line of dialogue).

## Expressions

Expressions are simply values ​​that you can obtain to store in a variable or use in a text string.

### Get dialogue line
![get_dialogue_line](/img/for_docs/expression_0.png)

Retrieves the current dialog line.

Example:
![get_dialogue_example](/img/for_docs/get_dialogue_example.png)

### Get who
![get_who](/img/for_docs/expression_1.png)

Get the character that is currently speaking.

Example:
![get_who_example](/img/for_docs/get_who_example.png)

### Get command parameter
![get_command_p](/img/for_docs/expression_4.png)

Obtain the parameter using its index from a custom command.

Example:
![get_command_parameter_example](/img/for_docs/get_command_parameter_example.png)

In your dialog file, you can have this command:
![code_command_parameter_example](/img/for_docs/code_command_parameter_example.png)

> [!NOTE]
> There are 4 numbers, each representing an index. The first number on the left is index 0, the second is 1, and so on.
> This expression must be used in conjunction with the "Command called" condition; otherwise, there will be undesirable results.

### Get options number
![get_option_number](/img/for_docs/expression_2.png)

Retrieves the number of available options.

Useful for creating radio buttons based on the number of options in an "option" block.

### Get option name
![get_option_name](/img/for_docs/expression_3.png)

Get the name of an option based on its index.

![get_option_name_example](/img/for_docs/get_option_name_example.png)

> [!NOTE]
> If you have 4 options, the first option has an index of 0, the second 1, and so on.