# firstAgent

Building my first AI agent with agent framework

I stepped upon cole medin's video [here](https://www.youtube.com/watch?v=U6LbW2IFUQw), he did a great job explaining how the 2 frameworks work to build an ai agent on your own. The two framework he used here are:

- Pydantic AI
- LangGraph

Install PydanticAI

```
pip install pydantic-ai
```

### Error and Resolutions

Following error while installing python3.13, as PydanticAI requires 3.9+ python.

BUILD FAILED (OS X 15.3.1 using python-build 20180424)

To fix the above on mac:

Uninstall the old tools
`$ sudo rm -rf /Library/Developer/CommandLineTools`

Reinstall Xcode Command line tools
`$ xcode-select --install`

Install python using pyenv
`$ pyenv install 3.8.5`

```
CFLAGS="-I$(brew --prefix openssl)/include" \
LDFLAGS="-L$(brew --prefix openssl)/lib" \
pyenv install -v 3.5.2
```

pyenv installing 3.9 kept not able to install correctly, it is due to mac m1, solution;
`brew install python3.9` and then establish the python3.9 in `.pyenv/versions`
