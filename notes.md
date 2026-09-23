## How to build it

To get around the permission limitations on shot:

in your gh repo:

- build quarto site (`quarto render`)
- then `scp -r quarto-build/ nsmith@shotaws.holycross.edu:xfer`


then on shotaws.holycross.edu:

```
cd xfer/quarto-build
sudo cp -r . $HOME/web
```