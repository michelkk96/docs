---
title: 個人アカウントからのユーザのブロック
intro: ユーザをブロックして、あなたのアクティビリティやリポジトリへのアクセスを拒否し、あなたに通知を送れないようにすることができます。
redirect_from:
  - /articles/blocking-a-user-from-your-personal-account
  - /github/building-a-strong-community/blocking-a-user-from-your-personal-account
versions:
  fpt: '*'
  ghec: '*'
topics:
  - Community
shortTitle: アカウントからのブロック
---

## ユーザのブロックについて

自分のアカウント設定、もしくはユーザのプロファイルからユーザをブロックできます。 {% data variables.product.prodname_dotcom %}は、ユーザをブロックしてもユーザに通知しません。 ブロックした人と同じプロジェクトにコントリビューションしたくない場合は、ブロックしたユーザがコントリビューションしているすべてのリポジトリで警告を表示させるように選択できます。 詳細は「[アカウント設定でのユーザのブロック](#blocking-a-user-in-your-account-settings)」を参照してください。 共有スペースでブロックされたユーザのアクティビティが引き続き表示される場合があり、ブロックされたユーザは既存のコンテンツを削除できます。

{% tip %}

**ヒント:**過熱した会話を鎮めるためにユーザをブロックする場合、会話をロックすることにより、コラボレータだけがコメントできるようになります。 詳細は「[会話をロックする](/communities/moderating-comments-and-conversations/locking-conversations)」を参照してください。

{% endtip %}

ユーザをブロックすると、以下のようになります:
- そのユーザによるあなたのフォローは止まります
- ユーザがリポジトリの Watch を停止し、リポジトリのピン留めを解除します
- そのユーザはあなたがオーナーの Organization には参加できなくなります
- そのユーザによる Star 付けや Issue 割り当てはリポジトリから削除されます。
- リポジトリ内のディスカッションまたはコメントに対するユーザの投票が削除されます
- そのユーザは、あなたのリポジトリのコラボレーターではなくなります
- リポジトリへのユーザのコントリビューションがカウントされなくなります
- ブロックされたユーザのリポジトリへのコントリビューションがカウントされなくなります
- リポジトリのコラボレータとして削除されます
- そのユーザの、あなたへのスポンサーシップはキャンセルされます
- ブロックされたユーザへの、またはブロックされたユーザからの保留中のリポジトリまたはアカウント継承者の招待がキャンセルされます
- The user is removed as a collaborator from all the projects and {% data variables.projects.projects_v1_boards %} owned by you
- You are removed as a collaborator from all the projects and {% data variables.projects.projects_v1_boards %} owned by the user

ユーザをブロックすると、ユーザは以下のことができなくなります:
- あなたのユーザ名の [@メンション](/articles/basic-writing-and-formatting-syntax/#mentioning-people-and-teams)を含む、あなたへの通知の送信
- 作成した Issue またはプルリクエストへのコメントまたは編集
- Issue、プルリクエスト、コミットに対するコメントへの反応
- あなたのフォロー、あるいはあなたのコンテンツを自身のアクティビティフィードで見ること
- Issue またはプルリクエストへの割り当て
- あなたを自身のリポジトリにコラボレーターとして招待すること
- あなた自身をセキュリティアドバイザリのコラボレータとして招待してください
- あなたのリポジトリをコメント中でクロス参照すること
- リポジトリのフォーク、Watch、ピン留め、Star 付け
- あなたをスポンサーすること
- Add you as a collaborator on their projects and {% data variables.projects.projects_v1_boards %}
- Make changes to your public projects and {% data variables.projects.projects_v1_boards %}

あなたが所有するリポジトリでは、ブロックされたユーザは以下のこともできなくなります:
- Issue のオープン
- プルリクエストの送信、クローズ、マージ
- Issue、プルリクエスト、あるいはコメントにコメントする
- ウィキページを追加または編集する

## アカウント設定でのユーザのブロック

{% data reusables.user-settings.access_settings %}
{% data reusables.user-settings.blocked_users %}
3. \[Block a user\] (ユーザをブロック) の下で、ブロックしたいユーザのユーザ名を入力し、[**Block user**] をクリックしてます。 ![ユーザ名フィールドとブロックボタン](/assets/images/help/settings/user-settings-block-user.png)
4. ブロックされたユーザがコントリビュータになっているリポジトリにアクセスした際に警告を表示させることもできます。それには [**Warn me when a blocked user is a prior contributor to a repository**] を選択します。 ![ブロックされたユーザについての警告オプション](/assets/images/help/settings/warn-block-user.png)

## プロフィールページでのユーザのブロック

{% data reusables.profile.user_profile_page_navigation %}
{% data reusables.profile.user_profile_page_block_or_report %}
3. [**Block user**] (ユーザをブロック) をクリックします。 ![ユーザのブロックあるいは悪用のレポートの選択肢を持つモーダルボックス](/assets/images/help/profile/profile-blockuser.png)

{% note %}

嫌がらせを受けた場合は、 {% data variables.contact.report_abuse %} を使用してご連絡ください。 {% data reusables.policies.abuse %}

{% endnote %}

## 参考リンク

- [個人アカウントからブロックしたユーザの表示](/communities/maintaining-your-safety-on-github/viewing-users-youve-blocked-from-your-personal-account)
- [個人アカウントからのユーザのブロック解除](/communities/maintaining-your-safety-on-github/unblocking-a-user-from-your-personal-account)
- [Organization からのユーザのブロック](/communities/maintaining-your-safety-on-github/blocking-a-user-from-your-organization)
- [Organization からのユーザのブロック解除](/communities/maintaining-your-safety-on-github/unblocking-a-user-from-your-organization)
- [悪用あるいはスパムのレポート](/communities/maintaining-your-safety-on-github/reporting-abuse-or-spam)
- 「[リポジトリでのインタラクションを制限する](/communities/moderating-comments-and-conversations/limiting-interactions-in-your-repository)」
