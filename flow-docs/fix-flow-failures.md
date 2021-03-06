---
title: フローのトラブルシューティング | Microsoft Docs
description: フローが失敗する最も一般的な理由のいくつかを解決します。
services: ''
suite: flow
documentationcenter: na
author: stepsic-microsoft-com
manager: anneta
editor: ''
tags: ''
ms.service: flow
ms.devlang: na
ms.topic: article
ms.tgt_pltfrm: na
ms.workload: na
ms.date: 01/17/2017
ms.author: stepsic
search.app:
- Flow
search.audienceType:
- flowmaker
- enduser
ms.openlocfilehash: 30efc05dad57bc86a99b90e849fd1c9459930e54
ms.sourcegitcommit: a20fbed9941f0cd8b69dc579277a30da9c8bb31b
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/12/2018
ms.locfileid: "44689481"
---
# <a name="troubleshooting-a-flow"></a>フローのトラブルシューティング
## <a name="identify-the-error"></a>エラーを特定する
フローを修正する前に、失敗した理由を明らかにする必要があります。 Web ポータルの上部にある通知アイコンをクリックまたはタップし (または、モバイル アプリの **[アクティビティ]** タブを開き)、表示される一覧でフローをクリックまたはタップします。

![通知](./media/fix-flow-failures/notifications-toolbar.png)

フローについての詳細が表示され、少なくとも 1 つのステップに赤い感嘆符アイコンが付いています。 そのステップを開き、エラー メッセージを確認します。

![エラー メッセージ](./media/fix-flow-failures/flow-run-failure.png)

## <a name="authentication-failures"></a>認証エラー
多くの場合、フローが失敗する原因は認証エラーです。 この種のエラーがある場合は、エラー メッセージに "**許可されていません**" という内容が含まれていたり、**401** または **403** のエラー コードが表示されたりします。 認証エラーは、通常、接続を更新することで解決できます。

1. Web ポータルの上部にある歯車アイコンをクリックまたはタップして **[設定]** メニューを開き、**[接続]** をクリックまたはタップします。
2. **許可されていません**というエラー メッセージが表示された接続に移動します。
3. 接続の横で、許可されていない接続に関するメッセージの **[パスワードの確認]** リンクをクリックまたはタップします。
4. 表示される指示に従って資格情報を確認し、フロー実行のエラーに戻って、**[再送信]** をクリックまたはタップします。
   
    フローが正常に実行されるようになります。

## <a name="action-configuration"></a>アクションの構成
フローのアクションの設定が意図したとおりに機能しない場合にも、フローは失敗します。 この場合、エラー メッセージに**無効な要求**または**見つかりません**といった言葉が含まれていたり、エラー コード **400** または **404** が表示されたりします。

エラー メッセージでは、エラーを修正する方法が指定されています。 **[編集]** ボタンをクリックまたはタップし、フロー定義内の問題を修正する必要があります。 更新したフローを保存し、**[再送信]** をクリックまたはタップして、更新した構成で再度実行を試みます。

## <a name="other-failures"></a>その他のエラー
エラー コード **500** または **502** が表示される場合は、一時的または過渡的な障害が発生しています。 **[再送信]** をクリックまたはタップして、フローをもう一度試みてください。

他の問題が発生した場合は、他のユーザーで同様の問題が発生している可能性があるため、[コミュニティに問い合わせてください](https://go.microsoft.com/fwlink/?LinkID=787467)。

