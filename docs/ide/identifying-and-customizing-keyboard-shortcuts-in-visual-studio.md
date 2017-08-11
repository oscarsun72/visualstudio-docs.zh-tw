---
title: "識別及自訂 Visual Studio 中的鍵盤快速鍵 | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "vs-ide-general"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "VS.ToolsOptionsPages.Environment.Keyboard"
helpviewer_keywords: 
  - "命令 [Visual Studio], 快速鍵"
  - "自訂快速鍵 [Visual Studio]"
  - "自訂鍵盤快速鍵 [Visual Studio]"
  - "匯出快速鍵 [Visual Studio]"
  - "匯入快速鍵 [Visual Studio]"
  - "鍵盤快速鍵 [Visual Studio], 自訂"
  - "快速鍵組合 [Visual Studio]"
ms.assetid: d2774be2-60a4-4d6f-95f1-79d0d9e55b56
caps.latest.revision: 26
author: "kempb"
ms.author: "kempb"
manager: "ghogen"
caps.handback.revision: 26
---
# 識別及自訂 Visual Studio 中的鍵盤快速鍵
[!INCLUDE[vs2017banner](../code-quality/includes/vs2017banner.md)]

您可以識別 Visual Studio 命令的鍵盤快速鍵、自訂這些捷徑，以及將它們匯出以供其他人使用。  許多捷徑會叫用相同的命令，不過，捷徑的行為可能會因為下列條件而不同：  
  
-   您在第一次執行 Visual Studio \(例如，一般開發或 Visual C\#\) 時選擇了哪些預設的環境設定。  
  
-   您是否曾自訂捷徑的行為。  
  
-   當您選擇捷徑時，是在使用什麼內容。  例如，如果您使用 \[設定設計工具\]，則 F2 捷徑會叫用 Edit.EditCell 命令，如果使用的是 \[Team Explorer\]，則會叫用 File.Rename 命令。  
  
 不論設定、自訂和內容為何，您一定可以在 \[**選項**\] 對話方塊中找到和變更鍵盤快速鍵。  您也可以在 [常用命令的預設鍵盤快速鍵](../ide/default-keyboard-shortcuts-for-frequently-used-commands-in-visual-studio.md)中查閱數十個命令的預設鍵盤快速鍵，您也可以在 [預設鍵盤快速鍵](../ide/default-keyboard-shortcuts-in-visual-studio.md) 中尋找所有預設捷徑的完整清單 \(以 \[一般開發設定\] 為基礎\)。  
  
 **本主題內容**  
  
-   [識別鍵盤快速鍵](../ide/identifying-and-customizing-keyboard-shortcuts-in-visual-studio.md#bkmk_identify)  
  
-   [自訂鍵盤快速鍵](../ide/identifying-and-customizing-keyboard-shortcuts-in-visual-studio.md#bkmk_assign)  
  
-   [共用自訂鍵盤快速鍵](../ide/identifying-and-customizing-keyboard-shortcuts-in-visual-studio.md#bkmk_transfer)  
  
 如果已在全域內容中將捷徑指派給某個命令，而且沒有其他內容，則該捷徑一定會叫用該命令。  不過，捷徑可以在全域內容中指派給某個命令，並在特定的內容中指派給不同命令。  如果您在特定內容中使用這類捷徑，該捷徑會叫用特定內容的命令，而不是全域內容的命令。  
  
> [!NOTE]
>  您的設定和 Visual Studio 版本可能會變更功能表命令的名稱和位置，以及出現在對話方塊中的選項。  本主題是以 \[**一般開發設定**\] 為基礎。  
  
##  <a name="bkmk_identify"></a> 識別鍵盤快速鍵  
  
1.  在功能表列上選擇 \[**工具**\]、\[**選項**\]。  
  
2.  展開 \[**環境**\]，然後選擇 \[**鍵盤**\]。  
  
     ![顯示 &#91;選項&#93; 對話方塊中的鍵盤快速鍵](../ide/media/optionskeyboard.png "OptionsKeyboard")  
  
3.  在 \[**顯示包含下列的命令**\] 方塊中，輸入沒有空格的所有或部分命令的名稱。  
  
     例如，您可以找到 solutionexplorer 的命令。  
  
4.  在清單中，選擇正確的命令。  
  
     例如，您可以選擇 \[**View.SolutionExplorer**\]。  
  
5.  如果命令已具有鍵盤快速鍵，則會出現在 \[**所選取命令的快速鍵**\] 清單中。  
  
     ![檢視所指定命令的捷徑](../ide/media/viewshortcut.png "ViewShortcut")  
  
##  <a name="bkmk_assign"></a> 自訂鍵盤快速鍵  
  
1.  在功能表列上選擇 \[**工具**\]、\[**選項**\]。  
  
2.  展開 \[**環境**\] 資料夾，然後選擇 \[**鍵盤**\]。  
  
     ![顯示 &#91;選項&#93; 對話方塊中的鍵盤快速鍵](../ide/media/optionskeyboard.png "OptionsKeyboard")  
  
3.  在 \[**顯示包含下列的命令**\] 方塊中，輸入沒有空格的所有或部分命令的名稱。  
  
     例如，您可以找到 solutionexplorer 的命令。  
  
4.  在清單中，選擇您要指派給鍵盤快速鍵的命令。  
  
5.  在 \[**新的快速鍵用於**\] 清單中選擇您要使用捷徑的功能區域。  
  
     例如，若要在所有的環境中使用該快速鍵，請選擇 \[**全域**\]。  您可以使用未在另一個編輯器中對應 \(為「全域」\) 的任何捷徑。  否則，編輯器會覆寫快速鍵。  
  
    > [!NOTE]
    >  您在 \[**全域**\] 中無法指派下列按鍵做為鍵盤快速鍵的一部分：Print Scrn\/Sys Rq、Scroll Lock、Pause\/Break、Tab、Caps Lock、Insert、Home、End、Page Up、Page Down、Windows 標幟按鍵、應用程式鍵，任一個方向鍵或 Enter、Num Lock、Delete 或數字鍵盤上的 Clear，或 Ctrl\+Alt\+Delete。  
  
6.  在 \[**按快速鍵**\] 方塊中，輸入您要使用的捷徑。  
  
    > [!NOTE]
    >  您可以建立組合字母與 Alt、Ctrl 或兩者的捷徑。  您也可以建立組合 Shift 鍵與字母，搭配 Alt、Ctrl 或兩者的捷徑。  
  
     如果已將該捷徑指派給其他命令，則該捷徑會出現在 \[**快速鍵目前已被下列命令所使用**\] 方塊中。  在這種情況下，請選擇退格鍵以刪除捷徑，再嘗試指派另一個捷徑。  
  
     ![為命令指定不同的捷徑](../ide/media/reassignshortcut.png "ReassignShortcut")  
  
7.  選擇 \[**指派**\] 按鈕。  
  
    > [!NOTE]
    >  如果您要為命令指定不同的快速鍵，請選擇 \[**指派**\] 按鈕，然後再選擇 \[**取消**\] 按鈕，此時對話方塊會關閉，但不會還原變更。  
  
##  <a name="bkmk_transfer"></a> 共用自訂鍵盤快速鍵  
 您可以將自訂鍵盤快速鍵匯出至檔案，再將檔案提供給其他人，讓其他人匯入資料，以共用您的自訂鍵盤快速鍵。  
  
#### 只匯出鍵盤快速鍵  
  
1.  在功能表列上，選擇 \[**工具**\]、\[**匯入和匯出設定**\]。  
  
2.  選擇 \[**匯出選取的環境設定**\]，然後選擇 \[**下一步**\] 按鈕。  
  
3.  在 \[**您要匯出哪一個設定?**\] 下方，取消選取 \[**所有設定**\] 核取方塊，展開 \[**選項**\]，然後展開 \[**環境**\]。  
  
4.  選取 \[**鍵盤**\] 核取方塊，然後選擇 \[**下一步**\] 按鈕。  
  
     ![僅匯出自訂的鍵盤快速鍵](../ide/media/exportshortcuts.png "ExportShortcuts")  
  
5.  在 \[**您要將設定檔命名為什麼?**\] 和 \[**在此目錄中儲存我的設定檔**\] 方塊中，保留預設值或指定不同的值，然後選擇 \[**完成**\] 按鈕。  
  
     根據預設，您的捷徑會儲存在 %USERPROFILE%\\Documents\\Visual Studio 2013\\Settings 資料夾的檔案中。  當您匯出設定時，檔案的名稱會反映日期，其副檔名為 .vssettings。  
  
#### 只匯入鍵盤快速鍵  
  
1.  在功能表列上，選擇 \[**工具**\]、\[**匯入和匯出設定**\]。  
  
2.  選擇 \[**匯入選取的環境設定**\] 選項按鈕，然後選擇 \[**下一步**\] 按鈕。  
  
3.  選擇 \[**否，只需匯入新設定並覆寫目前設定**\] 選項按鈕，然後選擇 \[**下一步**\] 按鈕。  
  
4.  在 \[**我的設定**\] 之下，選擇包含您要匯入之捷徑的檔案，或選擇 \[**瀏覽**\] 按鈕尋找正確的檔案。  
  
5.  選擇 \[**下一步**\] 按鈕。  
  
6.  在 \[**您要匯入哪一個設定?**\] 下方，取消選取 \[**所有設定**\] 核取方塊，展開 \[**選項**\]，然後展開 \[**環境**\]。  
  
7.  選取 \[**鍵盤**\] 核取方塊，然後選擇 \[**完成**\] 按鈕。  
  
     ![僅匯入自訂的鍵盤快速鍵](../ide/media/importshortcuts.png "ImportShortcuts")  
  
## 請參閱  
 [Visual Studio 的協助工具功能](../ide/reference/accessibility-features-of-visual-studio.md)
