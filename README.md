# MMM-SpaceLaunchNow

This is a module for [MagicMirror²](https://github.com/MichMich/MagicMirror/).

This module will show all recent or future launches bases on the SpaceLaunchNow API. I'm still working on expanding the module with additional information and options. If you have nice ideas, then you should certainly pass them on.

## Installation
1. Navigate to your MagicMirror's modules folder, and run the following command: `git clone https://github.com/koxm/MMM-SpaceLaunchNow.git`
2. Add the module and a valid configuration to your `config/config.js` file

## Using the module

This is an example configuration for your `config/config.js` file:
```js
var config = {
    modules: [
        {
            module: "MMM-SpaceLaunchNow",
            position: "middle_center",
            config: {
                records: 8,
                modus: "upcoming",
                showExtraInfo: true,
		        showColumnHeader: true,
	    }
	},
    ]
}
```

## Configuration options

| Option            | Description
|-------------------|--------------------------------------------
| `records`         | *Optional* - The number of lines you want to show <br>*Default:* 5
| `modus`           | *Optional* - 'past' for past launches, 'upcoming' for future launches <br>*Default:* past
| `showExtraInfo`   | *Optional* - Do you want to show the launchsite (true) or not (false) <br>*Default:* false
| `showColumnHeader`| *Optional* - Choose if you want to see columnheadings <br>*Default:* false

## Screenshot

This is a screenshot with extra info on false. Looks best on a left or right region. 
![Screenshot](https://github.com/koxm/MMM-SpaceLaunchNow/blob/master/Screenshot%201.png)

This is a screenshot with extra info on true. Looks better on a wider region, for example middle_center of bottom_bar.
![Screenshot](https://github.com/koxm/MMM-SpaceLaunchNow/blob/master/Screenshot%202.png)
