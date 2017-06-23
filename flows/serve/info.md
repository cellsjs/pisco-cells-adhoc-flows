# Flow serve

**'serve'** flow adapted for the command line interface, with an initial wizard to inquire the parameters.

## Steps

The steps of this flow are defined in the [configuration file][1]. This is the fragment of its configuration:

```json
{
  "serve-configure": {},
  "provide": {
    "type": "flow"
  },
  "build": {
    "type": "flow"
  },
  "launch": {
    "type": "flow"
  }
}
```

So we have a [`serve-configure`][2] step, and a [`provide`][3], [`build`][4] and [`launch`][5] flows.

### <a name="serve-configure"></a>serve-configure step

At this moment we will configure all the variables of the serve flow which are selectables for the user.
For example, in a context of an app, we can choose the kind of distribution we want to serve of the app (vulcanize,
 no vulcanize, for developoing).


### <a name="provide"></a>provide flow

The provide flow (second step of the serve flow). It will provide and install all dependencies and requirements. 
It is documented in [this page][6] of the [pisco-gitflow-flows][7] project.

### <a name="build"></a>build flow

Flow used in order to build sotware. Its documentation is allocated [here][8].

### <a name="launch"></a>launch flow

The final step will launch the context generated previously locally. The flow documentation is [here][9].


[1]: ./config.json
[2]: (#serve-configure)
[3]: (#install)
[4]: (#build)
[5]: (#launch)
[6]: https://github.com/cellsjs/pisco-gitflow-flows/blob/master/flows/provide/info.md
[7]: https://github.com/cellsjs/pisco-gitflow-flows
[8]: https://github.com/cellsjs/pisco-gitflow-flows/blob/master/flows/build/info.md
[9]: ../launch/info.md

