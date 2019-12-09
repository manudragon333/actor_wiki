<br/><br/>

> ### **Standard Behaviors in Actor Pattern (base.actor.js):**
1. Loader
1. Processor
1. Renderer
1. Responder
1. Composer
1. Validator
1. Performer
1. Director
***

> ### Running Karma Tests from Local:
## For HERO
For running only in Chrome Browser and also keep the browser waiting so that  
subsequent "Saves" on the file trigger tests automatically:  
`./node_modules/karma/bin/karma start karma-directives.conf.js --browsers Chrome`

For running once in all browsers and exiting:  
`./node_modules/karma/bin/karma start karma-directives.conf.js --single-run`

For running once in Chrome browser and exiting:  
`./node_modules/karma/bin/karma start karma-directives.conf.js --single-run --browsers Chrome`

Running a single describe or it block use `describe.only` or `it.only`

## For HYSB
For running once in Chrome browser and exiting:  
`./node_modules/karma/bin/karma start clientJasmine.conf.js --single-run --browsers Chrome`

***
> ### Running Mocha Tests from Local:
## For HERO
For running only in Chrome Browser and also keep the browser waiting so that  
subsequent "Saves" on the file trigger tests automatically:  
`./node_modules/karma/bin/karma start karma-mocha.conf.js --browsers Chrome`

For running once in all browsers and exiting:  
`./node_modules/karma/bin/karma start karma-mocha.conf.js --single-run`

For running once in Chrome browser and exiting:  
`./node_modules/karma/bin/karma start karma-mocha.conf.js --single-run --browsers Chrome`

Running a single describe or it block use `describe.only` or `it.only`

## For HYSB
For running once in Chrome browser and exiting:  
`./node_modules/karma/bin/karma start clientMocha.conf.js --single-run --browsers Chrome`
***
> ### Running IE11 Mocha Tests from Local:
`./node_modules/karma/bin/karma start karma-mocha.conf.js  --browsers=sl_ie_11 --sauce=true --hostname=<HOST_IP_ADDR>  --single-run`

**Note:** If connected via VPN, then the <HOST_IP_ADDR> should be the _**Virtual-IP**_ assigned by the VPN software.

***
> ### **Webstorm External Tools Configuration**
[Click here for instructions]

***
> ### How to override a specific locale in localhost for testing ?
Set a **_SESSION_** cookie as below:  
_CookieName_ = **Co.context.request.userLocale**  
_CookieValue_ = **localeString**  
Example:  
* `document.cookie="Co.context.request.userLocale=es_MX;path=/"; //Spanish Mexico`
* `document.cookie="Co.context.request.userLocale=es_US;path=/"; //Spanish US`
* `document.cookie="Co.context.request.userLocale=fr_CA;path=/"; //French Canada`

***
> ### **CMS Sharing State**
* **`ReadOnly`**: Dealer cannot make any changes to this content-record if its not a self owned record.
* **`Default`**: Dealer can create a clone from the parent content-record, _inheritance_ is not maintained.
* **`Extendable`** : Dealer can extend a record from parent content-record and _inheritance_ is maintained.
* **`Duplicate`**: It is just a copy of another record, no concept of parent-child.
<img src="cms_sharing_state_map.png" />

***


> ### **List of service-endpoints:**  

Put debug in the file /hydra-core/server/agent/base/Co.agent.base.js  
first line inside the IIFE and look for property `serviceAgents`.

Example:

<img src="endpoints_61bld85u8wk.png" />

***

> ### **Figure out the service endpoints from Hydra:**

In WebStorm put a breakpoint at "`Agent.request`" function in file:  
**/hydra-dev/src/node_modules/hydra-core/server/util/Co.util.agentV2.js**  
and print to console the value of _**`config.path`**_
***

> ### **Spec Runner Command:**  

`/Users/<username>/.nvm/versions/node/v8.7.0/bin/node /Users/<username>/StashWorkspace/hydra-dev/node_modules/jasmine-node/lib/jasmine-node/cli.js --verbose --captureExceptions --config HYDRA_CONFIG ./test/resources/hydra.json --config HYDRA_PROPS ./test/resources/hydra.properties /Users/<username>/StashWorkspace/hydra-dev/src/node_modules/hydra-site-builder/base/actor/composer/sb.composer.properties.spec.js`

***