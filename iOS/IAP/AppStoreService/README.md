# App Store Service

  有關 IAP，Apple 提供的 Server 服務，一般是後端會用到的服務

---

## 大綱

- [App Store Service](#app-store-service)
  - [大綱](#大綱)
  - [App Store Server Notifications](#app-store-server-notifications)
  - [App Store Connect API](#app-store-connect-api)
  - [參考](#參考)

---

## App Store Server Notifications

App Store 的通知，有些內容的異動會透過此 Server 來發送通知。

比如 Receipts 異動 :

印象中有類似[使用者退款]，[停止訂閱]這類的訊息，

細節請看[官網說明][App Store Server Notifications | Apple Developer Documentation]。

**相關連結 :**

- [App Store Server Notifications | Apple Developer Documentation]

- [Enabling App Store Server Notifications | Apple Developer Documentation]

- [responseBody | Apple Developer Documentation]

---

## App Store Connect API

可透過此服務知道 App 於 App Store Connect 上面的一些資訊。

會知道這個是因為後端有個需求需要知道 product id 對應的 price，

那時找到[這篇文章][app store connect - how to get price of an in app purchase item on my server using product id - Stack Overflow]。

裡面有提到 [App Store Connect API][App Store Connect API | Apple Developer Documentation] 有提供這樣的服務，

不過細節要去看提供哪些功能了。

**相關連結 :**

- [app store connect - how to get price of an in app purchase item on my server using product id - Stack Overflow]

- [App Store Connect API | Apple Developer Documentation]

- [Creating API Keys for App Store Connect API | Apple Developer Documentation]

---

## 參考

**App Store Server Notification :**

- [Enabling App Store Server Notifications | Apple Developer Documentation]

- [responseBody | Apple Developer Documentation]

**App Store Connect API :**

- [app store connect - how to get price of an in app purchase item on my server using product id - Stack Overflow]

- [App Store Connect API | Apple Developer Documentation]

- [Creating API Keys for App Store Connect API | Apple Developer Documentation]

<!-- 連結設定 -->

[App Store Server Notifications | Apple Developer Documentation]: https://developer.apple.com/documentation/appstoreservernotifications

[Enabling App Store Server Notifications | Apple Developer Documentation]: https://developer.apple.com/documentation/storekit/in-app_purchase/subscriptions_and_offers/enabling_app_store_server_notifications

[responseBody | Apple Developer Documentation]: https://developer.apple.com/documentation/appstoreservernotifications/responsebody

[App Store Connect API | Apple Developer Documentation]: https://developer.apple.com/documentation/appstoreconnectapi

[app store connect - how to get price of an in app purchase item on my server using product id - Stack Overflow]: https://stackoverflow.com/questions/65004506/how-to-get-price-of-an-in-app-purchase-item-on-my-server-using-product-id#

[Creating API Keys for App Store Connect API | Apple Developer Documentation]: https://developer.apple.com/documentation/appstoreconnectapi/creating_api_keys_for_app_store_connect_api

---

[=> Top](#app-store-service)

[=> Go Back](../README.md)
