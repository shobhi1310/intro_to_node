# Debugging

Did not cover it that much as it would be just a bunch of screenshots.

We can do debugging by:

1. Console logging at every place possible3
2. Use break points and debuggging tool built into VS Code
3. Go the smart way using Chrome's v8 engine

## Smart Way

Run

`node --inspect-brk [name of the file]`

After that go to your `chrome://inspect` on your browser and click on the available target you get on your browser.

This will open an instance of Chrome Dev tools and help in all the debugging techniques at particular break points. very resourceful!!

# Navigation Link
- [Deployment](./deployment.md)