# metachain Docs

metachain Docs, built with docusaurus; docs are live at https://developer.metachain-i.co/. 

[metachain SDK](https://github.com/META-MetaChain/metachain-sdk) auto-genned docs are included as submodule.

## Contribution

For most of the docs content, you can contribute by simply reviewing our [docs contribution guidelines](https://docs.metachain-i.co/for-devs/contribute) and opening a PR! 

The following are the only exceptions: 

- Contributing to the three troubleshooting pages — [nodes](metachain-docs/partials/_troubleshooting-nodes-partial.md), [builders](metachain-docs/partials/_troubleshooting-building-partial.md), and [users](metachain-docs/partials/_troubleshooting-users-partial.md), as well as the [glossary](metachain-docs/partials/_glossary-partial.md) page — requires internal Offchain Labs access. If you'd like to make a suggestion about content on any of those pages, open an [issue ticket](https://github.com/META-MetaChain/metachain-docs/issues).

- To request to have your project added to the [3rd party node providers page](metachain-docs/node-running/node-providers.mdx), use [this form](https://docs.google.com/forms/d/e/1FAIpQLSdw0U-9LcLuih5TZ_QghS-S_MS4wCKSEigA_IQEza_hFmNVow/viewform).


### Initial set up

```shell
git clone git@github.com:META-MetaChain/metachain-docs.git

cd metachain-docs/

git submodule update --init --recursive

cd website/
```

Install node dependencies
```
yarn
```

You will only need to generate docs once:
```
yarn generate_sdk_docs
```

### Dev Build

Live build without generating sdk docs (recommended):

```
yarn start_nitro_docs 
```


(Re)generate sdk docs and live build:
```
yarn start
```


### Update submodules

Sdk repo: 
```
git submodule update --remote metachain-sdk
```
