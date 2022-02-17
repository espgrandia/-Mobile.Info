# bundletool

---
---

## 大綱

- [bundletool](#bundletool)
  - [大綱](#大綱)
  - [說明](#說明)
    - [概述](#概述)
    - [下載 bundletool](#下載-bundletool)
      - [bundletool 格式](#bundletool-格式)
      - [命名別名配置](#命名別名配置)
  - [參考](#參考)

---
---

## 說明

### 概述

摘錄自[官網][bundletool  |  Android 开发者  |  Android Developers] :

bundletool 是一種底層工具，

可供 Android Studio、Android Gradle 插件和 Google Play 用於構建 Android App Bundle 文件並將 app bundle 轉換為部署到設備的各種 APK。

您也可以將 bundletool 作為一種命令行工具，

用於自行構建 app bundle 和重新創建應用 APK 的 Google Play 服務器端 build。

---

### 下載 bundletool

可自 [GitHub bundletool Release][Releases · google/bundletool · GitHub] 下載。

#### bundletool 格式

由於 bundletool 工具為一個 .jar 格式文件。

所以運行環境需要先配置 jaba 環境。

可使用 java -jar bundletool-xxx.jar 來使用。

#### 命名別名配置

另外，可使用腳本並配置環境變量，方便全局使用。

可參考 [bundletool 工具使用 - 簡書] 文章中，關於命令別平配置的方式。

![bundletool_alias](pics/bundletool_alias.png)

**bundletool alais for mac :**

這邊介紹 mac 的設定使用方式。

> windows 我沒有實驗，但應該也是可行的。

- 01 : 下載的 bundletool-xxx.jar 放到想要設定的資料夾中。

  ![01](pics/bundletool_alais_01.png)

- 02 : 測試 java -jar bundletool-xxx.jar

  確定可以使用該 bundletool-xxx.jar 工具。

  ![02](pics/bundletool_alais_02.png)

- 03 : mac 開啟 .bash_profile 或 .zshrc 檔案。

  開啟 mac 的環境設定檔案，於 macOS 10.6 之後，Apple 改使用 zsh shell 當期預設的 shell。

  ![03](pics/bundletool_alais_03_mac_zshrc_original.png)

- 04 : 新增別名的設定 (for .bash_profile or .zshrc)

  可設定如下 :

  以下為範例，可視個別需求，設定到合適的位置。

  ```shell
  alias bundletool="java -jar /Users/xxx/Desktop/Lib/bundletool/bundletool-all-1.8.2.jar"
  ```

  ![04](./pics/bundletool_alais_04_mac_zshrc_add_alias_content.png)

- 05 : 在 terminal 使環境變數立即生效。

  可使用 source .bash_profile or .zshrc ，使環境變數立即生效。

  ![05](./pics/bundletool_alais_05_mac_execute_source_zshrc.png)

- 06 : 驗證 alias

  ![06](./pics/bundletool_alais_06_mac_test_bundletool_alias_cmd_tool.png)

---
---

## 參考

- [bundletool  |  Android 开发者  |  Android Developers]

  官方說明。

- [Releases · google/bundletool · GitHub]

  bundletool 官方的下載位置。

- [bundletool 工具使用 - 簡書]

---

<!-- 連結設定 -->

[bundletool  |  Android 开发者  |  Android Developers]:
  [bundletool](https://developer.android.com/studio/command-line/bundletool#generate_apks)

[Releases · google/bundletool · GitHub]:
  https://github.com/google/bundletool/releases

[bundletool 工具使用 - 簡書]:
  https://www.jianshu.com/p/0308ddc9b2e7

---

[=> Top](#bundletool)

[=> Go Back](../README.md)
