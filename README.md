## Community Frame

> Updatable, democratic permaweb applications 📜

### About
Powered by Community.xyz SmartWeave contracts, people can propose votes in their DAOs to initialize and configure extra settings. One of these settings could set the content of the community's permawebb app. By deploying a static site that automatically loads this setting in the latest contract state (called a community frame), developers can build permaweb applications that update whenever the DAO votes to change the site content.

### How it works
The community frame works by loading the latest state of a given SmartWeave contract and setting an `iframe` element with the transaction hash in the setting: `siteDeployment`.

### Configuration
Configuring the community frame is extremely easy, as the codebase only consists of a 95-line `index.html` file. 

**Steps to configure**:

1. Fork this repository
2. Change the contract string on `index.html` at line 24
3. Update the default state of the site on line 34 in `index.html`