# indu.guru

![indu.guru](img/title.png)

## Setup

Before training the agents we need to install appropriate version of python and pip if not already installed.

```shell
# MacOS
> brew install python@3.9
```

When the appropriate version of python is installed then Update the pip3 package manager to the latest version.

```shell
> python3.9 -m pip install --upgrade pip
```

Now that you have the proper versions of python and pip installed let's setup the virtual environment. For more information on python virtual environments please see the [documentation](https://docs.python.org/3/library/venv.html).

```shell
> python3.9 -m virtualenv venv
> source ./venv/bin/activate
```

## Agent

Rasa is an open source conversational AI platform that allows you to understand and hold conversations. It supplies the building blocks for creating virtual assistants or chatbots.

Once your sytem environment is setup correctly we are going to install `Rasa`.

```shell
> python -m pip install rasa
```

The Agent is already initializes, so once Rasa is installed we can run any number of shell commands to interact.

### Training

Train the Agent using NLU data and stories, saves trained model in `./models`.

```shell
> rasa train
```

Start an interactive learning session to create new training data by chatting with the Agent.

```shell
> rasa interactive
```

Load the Agent and talk on the command line.

```shell
> rasa shell
```

Starts a server with the Agent.

```shell
> rasa run --enable-api
```

Generates a visual representation of your stories.

```shell
> rasa visualize
```

---

[Github Repo](https://github.com/indraai/indu.guru)  
[Back to indra.ai](https://indra.ai)  
&copy;2022 Quinn Michaels; All Rights Reserved.
