# Getting Started Guide 💡

This guide is designed to help you quickly understand the concepts of Sakura Dialog System.

## Requisitos

- Instala la ultima versión de GDevelop
- Instala la ultima versión de Visual Studio Code
- Download the Sakura Script extension from [here](https://github.com/QuetzalcoutlDev/sakura-script/releases/).
- Download and install the Sakura Dialog System extension in your project [download it here](https://github.com/QuetzalcoutlDev/SakuraDialogSystemGD/releases/)

# Condiciones y acciones

Una vez que cumples todos los requisitos, podemos comenzar con las explicaciones sobre las condiciones y acciones

Si no haz instalado la extensión, simplemente abre el menú lateral de GDevelop y haz clic en el botón + del apartado "Extensiones"
![how_to_install](/img/for_docs/how_to_install.png)

Haces clic en "importar extensión" y buscas la extensión de Sakura Dialog System que descargaste.

Si instalaste la extensión correctamente, deberias ver reflejado "Sakura Dialog System" en el menú de condiciones y acciones
![conditions](/img/for_docs/in_conditions.png) ![actions](/img/for_docs/in_actions.png)

## Condiciones

Las condiciones son como preguntas internas que hace GDevelop a la extensión para ver si lo que le estas preguntando es verdadero, por ende, realizar algo, y si es falso, también realizar algo (si quieres).

### Dialog is running
![running](/img/for_docs/condition_0.png)

Comprueba que el dialogo se está ejecutando.

### Get line type
![line](/img/for_docs/condition_1.png)

Obtiene el tipo de linea actual que puede ser: "dialogue", "options", "command", "conditionals"

Puedes hacer que se haga una acción si una de esas lineas está.

### Command called
![called](/img/for_docs/condition_2.png)

Obtiene el nombre del comando personalizado y permite obtener sus parametros.

## Acciones

Las acciones son eventos que se deben realizar si una condición se cumple o que siempre deben realizarse.

### Load dialog file
![load_dialog](/img/for_docs/action_0.png)

Carga un archivo de dialogo en formato .json, exportado desde Visual Studio Code.

Todas las acciones y condiciones se podrán ejecutar, una vez se use está acción antes de todo.

![load_file_example](/img/for_docs/load_file_example.png)
> [!NOTE]
> Evita a toda costa, hacer clic en "Crear/Editar con Yarn" ya que de otro modo fallara el sistema de dialogo ya que Yarn no es compatible con el formato de dialogo de Sakura Script.

### Go to branch
![go_to_branch](/img/for_docs/action_1.png)



### Go to next line
![next_line](/img/for_docs/action_2.png)

### Confirm option selection
![confirm_option](/img/for_docs/action_3.png)

### Stop dialogue
![stop_dialogue](/img/for_docs/action_4.png)

### Save State
![save_state](/img/for_docs/action_5.png)

### Load State
![load_state](/img/for_docs/action_6.png)

## Expresiones

Faltan las expresiones, que no son más que valores que puedes obtener para guardar en una variable o usarlo en una cadena de texto.

### Get dialogue line
![get_dialogue_line](/img/for_docs/expression_0.png)

![get_dialogue_example](/img/for_docs/get_dialogue_example.png)

### Get who
![get_who](/img/for_docs/expression_1.png)

![get_who_example](/img/for_docs/get_who_example.png)

### Get command parameter
![get_command_p](/img/for_docs/expression_4.png)

![get_command_parameter_example](/img/for_docs/get_command_parameter_example.png)

### Get options number
![get_option_number](/img/for_docs/expression_2.png)

### Get option name
![get_option_name](/img/for_docs/expression_3.png)

![get_option_name_example](/img/for_docs/get_option_name_example.png)