# firstAgent

Building my first AI agent with agent framework

I stepped upon cole medin's video [here](https://www.youtube.com/watch?v=U6LbW2IFUQw), he did a great job explaining how the 2 frameworks work to build an ai agent on your own. The two framework he used here are:

- Pydantic AI
- LangGraph

Install PydanticAI

```
pip install pydantic-ai
```

Docker is also required

### Architecture

- PydanticAI: connect to LLM
- Docker Build

### Error and Resolutions

Following error while installing python3.13, as PydanticAI requires 3.9+ python.

BUILD FAILED (OS X 15.3.1 using python-build 20180424)

To fix the above on mac:

1. delete all python versions (using `brew uninstall`)
2. Uninstall the old tools
   `$ sudo rm -rf /Library/Developer/CommandLineTools`
3. Reinstall Xcode Command line tools
   `$ xcode-select --install`
4. Install python using pyenv
   `$ pyenv install 3.13`

After above new error: WARNING: Disabling truststore since ssl support is missing

4. Please also make sure `gcc` has been installed successfully

5. What ultimately resolved it is using the solution from; https://github.com/pyenv/pyenv/issues/993

6. run `source .zshrc` or `exec .zshrc -l`

7. close terminals & reopen to reset everything

alternatively for temporary fixes:
pyenv installing 3.9 kept not able to install correctly, solution;
`brew install python3.9` and then establish the python3.9 in `.pyenv/versions`
