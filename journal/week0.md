# Week 0 — Billing and Architecture

## Required Homework

### Install and Verify AWS CLI 

Installed the AWS CLI for Windows, because of the [AWS CLI Instruction Documentation Page](https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html) that was clear and this made installing it a breeze. Below you will find the command I used to install the AWS CLI on a Windows computer.

```
msiexec.exe /i https://awscli.amazonaws.com/AWSCLIV2.msi
```
Below I have also attach a screenshot of how I installed it locally on my machine and with a few command attached.

When opening **Command Prompt** press `windows key + r`, you will find the Windows key on a Windows keyboard.

![Opening CMD on windows](assets/week-0-command%20prompt.png)

If this window appear, type in `cmd` and press the `enter` key on your keyboard.

Installing the AWS CLI you need to paste the command and then press `enter` to install.

![Show AWS CLI is installed](assets/week-0-installing%20aws%20cli.png)

When Done installing it will show it is unable to find the problem, a quick fix for me was to read the [Troubleshooting AWS CLI errors](https://docs.aws.amazon.com/cli/latest/userguide/cli-chap-troubleshooting.html) and found that I just need to restart my command prompt.

![Showing installed AWS CLI](assets/week-0-show%20aws%20cli%20is%20installed.png)

Another roadblock when wanting to see check if my AWS identy is showing in cli. It was not showing because I used my **IAM user** credentials to log in and not **Access key** and the **Secret access key**.

![Proof of logged in on AWS CLI](assets/week-0-using%20sts%20identity.png)

### Create a Budget

I created my own Budget for $10, the reason I can not afford any spent more then it. I also created another budget but delete the budget because I did'nt want to have a second one. I also know that you can only create 2 free budget limit anything above the limit will result in a extra fee.

![image of The Budget Alarm I Created](assets/week-0-budget%20alarm.png)

### Recreate Logical Architecture Design

Creating the logical diagram wasn't difficult but doing research on [AWS Architecture](https://aws.amazon.com/architecture/) helped alot in understanding each piece that fits onto the diagram. 

![Cruddur Logical Design](assets/week-0-aws%20logical%20diagram.png)

## Homework Challanges
