---
标题：分叉存储库
allowTitleToDifferFromFilename:true
重定向(_F)：
-/fork-a-repo
-/分叉
-/articles/fork-a-repo
-/github/github入口/fork-a-repo
-/github/getting-started-with-github/quickstart/fork-a-repo
-/get-started/quickstart/fork-a-repo
简介：分叉是一个新的存储库，它与原始的“上游”存储库共享代码和可见性设置。
权限：“{%数据可重用。企业帐户。emu-permission-fork%}"
版本：
FPT：'*'
GHEs：'*'
ghec：'*'
主题：
-拉取请求
-问题
-通知
-帐户
---
##关于叉

{%数据可重用。reposits.fork-definition-long%}有关详细信息，请参阅[AUTOTITLE](/拉式请求/用拉式请求协作/用叉工作).

###建议对其他人的项目进行更改

例如，您可以使用分叉来建议与修复Bug相关的更改.您可以：

*将存储库分叉。 将存储库分叉。
*进行修复。搞定。
*向项目所有者提交提取请求。 向项目所有者提交提取请求。

###用别人的项目作为自己想法的起点。 把别人的项目作为你自己想法的起点。

开源软件基于这样的理念：通过共享代码，我们可以制作更好、更可靠的软件。 有关更多信息，请参阅[关于开源计划](关于开源计划的https://opensource.org/about))。[关于开源计划](https://opensource.org/about)关于开源计划。

有关将开放源代码原则应用于组织对{%data variables.product.prodname_dotcom%}的开发工作的详细信息，请参阅{%data variables.product.prodname_dotcom%}的白皮书[内部资源简介](https://resources.github.com/whitepapers/introduction-to-innersource/).[内部资源简介](https://resources.github.com/whitepapers/introduction-to-innersource/).

从某人的项目分支创建公共存储库时，请确保包含一个许可证文件，以确定您希望如何与其他人共享项目。 有关详细信息，请参阅[选择开放源代码许可证](https://choosealicense.com/)位于choosealicense.com。[选择开放源代码许可证](https://choosealicense.com/)在choosealicense.com。

{%数据可重复使用。 开源。 开源指南存储库%}{%数据可重用。 开源。 开源学习%}

##前提条件先决条件

如果尚未设置Git，请首先使用Git中的{%data variables.location.product_location%}设置Git和身份验证.有关详细信息，请参阅[AUTOTITLE](/get-started/git-basics/set-up-git)。[AUTOTITLE](/get-started/git-basics/set-up-git).

##分库分叉存储库

{%webui%}

您可以将项目分叉，以建议对上游存储库进行更改。在这种情况下，定期将分叉与上游存储库同步是一种很好的做法。为此，您需要在命令行上使用Git.您可以使用刚刚分叉的[Octocat/匙刀](https://github.com/octocat/Spoon-Knife)存储库)来练习设置上游存储库。[Octocat/匙刀](https://github.com/octocat/Spoon-Knife)您刚刚分叉的存储库。

1.在{%ifversion fpt或ghec%}{%个数据变量上。product.prodname_dotcom%}{%else%}{%数据变量。location.product_location%}{%endif%}，导航到[Octocat/匙刀](https://github.com/octocat/Spoon-Knife)存储库)。在{%ifversion fpt或ghec%}上{%个数据变量。Product.prodname_dotcom%}{%else%}{%个数据变量。location.product_location%}{%endif%}，导航到[Octocat/匙刀](https://github.com/octocat/Spoon-Knife)存储库。
1.在页面右上角，单击**叉**。 在页面的右上角，单击**叉**.

！[存储库主页面的屏幕截图。 一个带有叉形图标和“叉形59.3k”的按钮以黑色显示橙。](/assets/images/help/repository/fork-button.PNG)![存储库主页面的屏幕快照。 一个按钮标有一个叉形图标和“叉形59.3k”，以深橙色显示。](/assets/images/help/repository/fork-button.PNG)
1.在“所有者”下，选择下拉菜单，然后单击分叉存储库的所有者。 在“所有者”下，选择下拉菜单，然后单击分叉存储库的所有者。
1.默认情况下，分叉的名称与上游存储库相同。 (可选)要进一步区分分叉，请在“存储库名称”字段中键入名称。 默认情况下，分叉的名称与上游存储库相同。 (可选)要进一步区分分叉，请在“存储库名称”字段中键入名称。
1.(可选)在“说明”字段中，键入分叉的说明。 或者，在“描述”字段中，键入您的叉的描述。
1.(可选)选择**仅复制默认分支**。(可选)选择**仅复制默认分支**.

对于很多分叉场景，例如参与开源项目，您只需要复制默认分支即可，如果不选择此选项，则所有分支都会被复制到新的分叉中。
1.单击**创建分叉**。单击**创建分叉**.

>[！注意] [！注意]
>如果要从上游存储库复制其他分支，可以从**分支**页面执行此操作。 有关详细信息，请参见[AUTOTITLE](/拉式请求/用拉式请求进行协作/用拉式请求为您的工作提出变更建议-请求/在存储库中创建和删除分支)。 如果要从上游存储库复制其他分支，可以从**分支机构**有关详细信息，请参阅[AUTOTITLE](/拉动式请求/拉动式请求协作/拉动式请求对工作提出更改/cr在您的存储库中吃掉并删除分支).

{%endwebui%}

{%cli%}

{%data reusables.cli.cli-learn-more%}

要创建存储库的分支，请使用'GH回购叉'子命令。`GH回购叉`子命令。

"'shellshell
GH回购叉库
```

要在组织中创建分支，请使用"--org"标志.'--组织标志.

"'shellshell
GH回购叉库--组织"octo-org"
```

{%endcli%}

{%desktop%}

您可以在{%个数据变量上派生存储库。产品。prodname_dotcom_the_web站点%}或在{%data variables.product.prodname_desktop%}中。有关在{%数据上分叉的信息，请参阅变量。产品。prodname_dotcom_the_web站点%}，请参阅[本文的Web浏览器版本](/pull-requests/使用pull-requests协作/使用forks/fork-a-repo？工具=webui)。[本文的Web浏览器版本](/pull-requests/使用pull-requests协作/使用forks/fork-a-repo？工具=webui).

{%data reusables.desktop.forking-a-repo%}

{%enddesktop%}

{%webui%}

##克隆分叉存储库克隆分叉存储库

现在，您有一个勺刀存储库的分支，但是您的计算机上没有该存储库中的本地文件。

1.在{%ifversion fpt或ghec%}{%个数据变量上。product.prodname_dotcom%}{%else%}{%数据变量。location.product_location%}{%endif%}，导航到**勺刀存储库的分叉**.在{%ifversion fpt或ghec%}上{%个数据变量。product.prodname_dotcom%}{%else%}{%个数据变量。location.product_location%}{%endif%}，导航到**你的叉子**勺子刀仓库的。
{%data reusables.reeposits.copy-clone-url%}
{%数据可重用。命令行。打开multi_os_terminal%}
{%数据可重用。命令行。更改-当前-目录-克隆(_L)%}
1.键入"git克隆"，然后粘贴先前复制的URL.它将如下所示，包含您的{%数据变量。product.github%}用户名而不是"您的用户名“”：类型`吉特克隆`，然后粘贴先前复制的URL。它将如下所示，包含您的{%数据变量。product.github%}用户名而不是`您的用户名`:

"'shell"'shell
git克隆https://{%数据变量。产品。product_url%}/您的用户名/spopper-Clifegit克隆https://{%数据变量。产品。product_url%}/您的用户名/勺子-克里夫
   ```

1. Press **Enter**. Your local clone will be created.

   ```shell
   $ git clone https://{% data variables.product.product_url %}/YOUR-USERNAME/Spoon-Knife
   > Cloning into `Spoon-Knife`...
   > remote: Counting objects: 10, done.
   > remote: Compressing objects: 100% (8/8), done.
   > remote: Total 10 (delta 1), reused 10 (delta 1)
   > Unpacking objects: 100% (10/10), done.
   ```

{% endwebui %}

{% cli %}

## Cloning your forked repository

Right now, you have a fork of the Spoon-Knife repository, but you do not have the files in that repository locally on your computer.

{% data reusables.cli.cli-learn-more %}

To create a clone of your fork, use the `--clone` flag.

```shell
gh repo fork REPOSITORY --clone=true
```

{% endcli %}

## Configuring Git to sync your fork with the upstream repository

When you fork a project in order to propose changes to the upstream repository, you can configure Git to pull changes from the upstream repository into the local clone of your fork.

{% webui %}

1. On {% ifversion fpt or ghec %}{% data variables.product.prodname_dotcom %}{% else %}{% data variables.location.product_location %}{% endif %}, navigate to the [octocat/Spoon-Knife](https://github.com/octocat/Spoon-Knife) repository.
{% data reusables.repositories.copy-clone-url %}
{% data reusables.command_line.open_the_multi_os_terminal %}
1. Change directories to the location of the fork you cloned.
    * To go to your home directory, type just `cd` with no other text.
    * To list the files and folders in your current directory, type `ls`.
    * To go into one of your listed directories, type `cd YOUR-LISTED-DIRECTORY`.
    * To go up one directory, type `cd ..`.
1. Type `git remote -v` and press **Enter**. You will see the current configured remote repository for your fork.

   ```shell
   $ git remote -v
   > origin  https://{% data variables.product.product_url %}/YOUR-USERNAME/YOUR-FORK.git (fetch)
   > origin  https://{% data variables.product.product_url %}/YOUR-USERNAME/YOUR-FORK.git (push)
   ```

1. Type `git remote add upstream`, and then paste the URL you copied in Step 3 and press **Enter**. It will look like this:

   ```shell
   git remote add upstream https://{% data variables.product.product_url %}/ORIGINAL-OWNER/Spoon-Knife.git
   ```

1. To verify the new upstream repository you have specified for your fork, type `git remote -v` again. You should see the URL for your fork as `origin`, and the URL for the upstream repository as `upstream`.

   ```shell
   $ git remote -v
   > origin    https://{% data variables.product.product_url %}/YOUR-USERNAME/YOUR-FORK.git (fetch)
   > origin    https://{% data variables.product.product_url %}/YOUR-USERNAME/YOUR-FORK.git (push)
   > upstream  https://{% data variables.product.product_url %}/ORIGINAL-OWNER/ORIGINAL-REPOSITORY.git (fetch)
   > upstream  https://{% data variables.product.product_url %}/ORIGINAL-OWNER/ORIGINAL-REPOSITORY.git (push)
   ```

Now, you can keep your fork synced with the upstream repository with a few Git commands. For more information, see [AUTOTITLE](/pull-requests/collaborating-with-pull-requests/working-with-forks/syncing-a-fork).

{% endwebui %}

{% cli %}

{% data reusables.cli.cli-learn-more %}

To configure a remote repository for the forked repository, use the `--remote` flag.

```shell
gh repo fork REPOSITORY --remote=true
```

To specify the remote repository's name, use the `--remote-name` flag.

```shell
gh repo fork REPOSITORY --remote-name "main-remote-repo"
```

{% endcli %}

### Editing a fork

You can make any changes to a fork, including:

* **Creating branches:** [_Branches_](/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-and-deleting-branches-within-your-repository) allow you to build new features or test out ideas without putting your main project at risk.
* **Opening pull requests:** If you want to contribute back to the upstream repository, you can send a request to the original author to pull your fork into their repository by submitting a [pull request](/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/about-pull-requests).

## Find another repository to fork

Fork a repository to start contributing to a project. {% data reusables.repositories.you-can-fork %} For more information about when you can fork a repository, see [AUTOTITLE](/pull-requests/collaborating-with-pull-requests/working-with-forks/about-permissions-and-visibility-of-forks).

{% ifversion fpt or ghec %}You can browse [Explore {% data variables.product.prodname_dotcom %}](https://github.com/explore) to find projects and start contributing to open source repositories. For more information, see [AUTOTITLE](/get-started/exploring-projects-on-github/finding-ways-to-contribute-to-open-source-on-github).

{% endif %}

## Next steps

You have now forked a repository, practiced cloning your fork, and configured an upstream repository.

* For more information about cloning the fork and syncing the changes in a forked repository from your computer, see [AUTOTITLE](/get-started/git-basics/set-up-git).

* You can also create a new repository where you can put all your projects and share the code on {% data variables.product.prodname_dotcom %}. {% data reusables.getting-started.create-a-repository %}

* {% data reusables.getting-started.being-social %}

* {% data reusables.support.connect-in-the-forum-bootcamp %}
