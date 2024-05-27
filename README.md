# @rounded-square/prettier-config

A configuration file for Prettier, used internally to ensure consistent code style among all company projects.

To use Prettier, install it globally on your system.

```
npm i -g prettier
```

Then, enable it in your IDE (https://prettier.io/docs/en/editors). Make sure to set Prettier as your **default formatter**.

----

### Usage

To use this package, add it to your project's ```package.json``` file.

First, install the package as a development dependency.

```
npm i @rounded-square/prettier-config -D
```

Then, reference it in the ```prettier``` property.

The end result should look something like this.

```
{
  "name": "some-project",
  "prettier": "@rounded-square/prettier-config",
  "devDependencies": {
    "@rounded-square/prettier-config": "x.y.z"
    ...
  },
  ...
}
```

Some IDEs (e.g. WebStorm) should be restarted after installing this package.

Now, every time you format the document in your IDE, styles from the package should be applied. **Do not create your own overriding styles (e.g. creating a new ```.prettierc``` file for the project)**. To read more about Prettier's code style philosophy, see [this](https://prettier.io/docs/en/why-prettier).

----

### Updates

```
npx npm-check-updates @rounded-square/prettier-config -u
npm i
```
