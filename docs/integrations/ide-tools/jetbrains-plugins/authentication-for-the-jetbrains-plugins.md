# Authentication for the JetBrains plugins

The first time you start a scan, the plugin automatically downloads the CLI in the background unless you have opted not to download automatically. To use the plugin you must authenticate. There are several ways to authenticate once the plugin is installed.

## Automatic authentication

After the CLI is installed, you are prompted to authenticate and connect the JetBrains plugin to Snyk.

![Prompt to authenticate and start testing your code.](<../../../.gitbook/assets/Screenshot 2022-02-10 at 17.07.52.png>)

Click **Test code now**. The plugin relies on the Snyk CLI, which authenticates your machine against the Snyk Web UI.

Click **Authenticate** when prompted by Snyk.

![Prompt to authenticate](../../../.gitbook/assets/screen-shot-2021-09-29-at-4.04.29-pm.png)

When authentication is complete, a confirmation message appears.

![Authenticated confirmation message](../../../.gitbook/assets/screen-shot-2021-09-29-at-4.05.55-pm.png)

The IDE reads and saves the authentication on your local machine.

You can now close the browser window and return to the IDE.

The analysis starts automatically:

![Analysis by JetBrains plugin](<../../../.gitbook/assets/Screenshot 2022-02-10 at 17.26.44.png>)

## Add token manually

1. Get your API token from your Snyk account: [https://app.snyk.io/account](https://app.snyk.io/account)
2. In the JetBrains plugin navigate to **Preferences** > **Tools** > **Snyk**.
3. Paste or enter the token under **Connect IDE to Snyk**.
4. Click **Apply** or **OK**.

![Connect IDE to Snyk token](../../../.gitbook/assets/screen-shot-2021-09-30-at-8.10.21-am.png)

## Manual authentication

If you are unable to authenticate automatically or by adding the token, run `snyk auth` from the command line and follow the preceding steps to respond to the prompts. If you need help, submit a request to [Snyk support](https://snyk.zendesk.com/agent/dashboard).

![Prompt from authentication using snyk auth](../../../.gitbook/assets/screen-shot-2021-09-29-at-3.57.26-pm.png)

##
