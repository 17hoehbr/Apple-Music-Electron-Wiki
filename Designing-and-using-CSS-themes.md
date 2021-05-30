### Designing your own CSS theme is pretty advanced so if your unable to do it then don't do it.
However, if you are indeed capable of making CSS themes you can use the template in the `assets/` in the source directory named `default_style.css`

## Using your CSS or pre-existing CSS themes.
Themes are capable of being chosen by either dropping your css file into the `assets/themes/` directory (if your making your own) or if your not you can just continue with the next step.

### Set the theme in the `config.json` file.
**Disclaimer: do not add the .css extension to the theme while inputting it into the `config.json` file.**

Open the `config.json` file in your respected text editor and find the `cssTheme` option as seen below

![cssTheme](https://i.imgur.com/HFxNifm.png)

Next, add your filename (not the extension just the filename) that you put into the `/assets/themes` folder if you made it yourself otherwise input the filename of a pre-existing theme in that folder and place it in-between the quotes.

After your done it should look like this.

![Finished CSS](https://i.imgur.com/XzO1xnV.png)

And your done! Recompile and see the changes.