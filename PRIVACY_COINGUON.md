# Chính sách quyền riêng tư — Cội Nguồn

*Cập nhật: 22/10/2026*

Cội Nguồn là ứng dụng gia phả cho dòng họ Việt trên iOS (App Store) và Android (Google Play), do GLab phát triển. Ứng dụng miễn phí, không quảng cáo, không bán hay cho thuê dữ liệu.

## Dữ liệu chúng tôi lưu

- **Tài khoản.** Khi đăng nhập bằng Google hoặc Apple, ứng dụng nhận tên hiển thị, email và mã định danh tài khoản từ nhà cung cấp. Với Apple, bạn có thể chọn ẩn email. Nếu chọn "Dùng ngay không cần tài khoản", ứng dụng chỉ tạo một mã định danh ẩn danh.
- **Gia phả do bạn và người thân nhập.** Họ tên, tên húy, tên tự, thụy hiệu, giới tính, đời, chi, quan hệ cha mẹ – vợ chồng – con, ngày sinh, ngày mất, ngày giỗ, địa chỉ mộ phần, ghi chú, ảnh chân dung, ảnh mộ. Với người còn sống có thể có thêm số điện thoại và địa chỉ.
- **Thông tin dòng họ.** Tên dòng họ, địa chỉ nhà thờ họ, danh sách tài khoản tham gia, vai trò của từng người, đề xuất sửa và lời mời.
- **Báo lỗi.** Khi ứng dụng gặp lỗi, Firebase Crashlytics ghi lại thông tin kỹ thuật: dòng máy, phiên bản hệ điều hành, phiên bản ứng dụng, nhật ký lỗi và mã cài đặt ngẫu nhiên. Báo lỗi không chứa nội dung gia phả.
- **Chống giả mạo.** Firebase App Check dùng Apple App Attest / DeviceCheck hoặc Google Play Integrity để xác nhận yêu cầu đến từ ứng dụng thật.

Ứng dụng **không** dùng công cụ phân tích hành vi, **không** theo dõi người dùng giữa các ứng dụng hay trang web, **không** đọc mã quảng cáo (IDFA, Android Advertising ID), **không** dùng vị trí, micro hay danh bạ.

## Dữ liệu dùng để làm gì

Chỉ để chạy các chức năng của ứng dụng: đăng nhập, lưu và đồng bộ gia phả giữa các thành viên, tính lịch giỗ, nhắc giỗ, mời người thân, và sửa lỗi ứng dụng.

## Ai xem được

- Gia phả là **riêng tư**: chỉ những tài khoản đã được mời vào dòng họ mới xem được.
- **Số điện thoại và địa chỉ** của người còn sống chỉ hiện cho Trưởng tộc, Biên tập chi và Thành viên. Vai trò Khách không xem được.
- Quyền sửa phụ thuộc vai trò: Trưởng tộc, Biên tập chi (chi của mình), Thành viên (gửi đề xuất sửa để Trưởng tộc duyệt).
- Chúng tôi không chia sẻ dữ liệu cho bên thứ ba nào khác ngoài nhà cung cấp hạ tầng bên dưới.

## Nơi lưu trữ

Dữ liệu được lưu trên **Google Firebase** (Authentication, Cloud Firestore, Crashlytics, App Check). Firestore đặt tại khu vực Singapore (`asia-southeast1`). Dữ liệu được mã hoá khi truyền (HTTPS/TLS) và khi lưu trên máy chủ của Google. Ứng dụng giữ bản sao gia phả trong bộ nhớ đệm trên máy để xem được khi mất mạng.

## Quyền trên thiết bị

- **Camera, Thư viện ảnh:** chỉ khi bạn chủ động chụp hoặc chọn ảnh chân dung, ảnh mộ. Ảnh được thu nhỏ trước khi lưu.
- **Thông báo:** nhắc ngày giỗ. Lời nhắc được lên lịch ngay trên máy.

## Thông tin về người khác

Gia phả chứa thông tin về người thân, kể cả người còn sống và trẻ em. Hãy chỉ nhập thông tin mà người đó (hoặc cha mẹ, người giám hộ của trẻ) đồng ý chia sẻ trong dòng họ. Người được nhắc đến có thể liên hệ Trưởng tộc hoặc chúng tôi để sửa hoặc xoá thông tin của mình.

Ứng dụng không hướng tới trẻ em dưới 13 tuổi và không cố ý thu thập dữ liệu từ trẻ em tự sử dụng ứng dụng.

## Thời gian lưu và cách xoá

- **Xoá tài khoản:** tab **Tôi → Xoá tài khoản**. Tài khoản đăng nhập và tư cách thành viên ở mọi dòng họ bị xoá ngay, không khôi phục được. Token đăng nhập Apple / Google cũng được thu hồi. Phần gia phả bạn đã nhập vẫn được giữ cho dòng họ vì đó là dữ liệu chung của cả họ. Nếu bạn là người duy nhất trong một dòng họ, dòng họ đó bị xoá cùng.
- **Xoá dòng họ:** Trưởng tộc có thể xoá toàn bộ dòng họ (phả, ảnh, lịch giỗ, danh sách thành viên) ở tab **Dòng họ → Thông tin**.
- **Xoá một người khỏi phả:** Trưởng tộc có thể xoá hồ sơ, ảnh và thông tin liên lạc của một người.
- Dữ liệu được giữ đến khi bị xoá theo các cách trên. Báo lỗi Crashlytics được Google tự xoá sau 90 ngày.
- Không xoá được trong ứng dụng? Gửi email cho chúng tôi, chúng tôi xử lý trong vòng 30 ngày.

## Quyền của bạn

Bạn có quyền xem, sửa, xoá dữ liệu của mình và rút lại sự đồng ý bất cứ lúc nào, theo Nghị định 13/2023/NĐ-CP về bảo vệ dữ liệu cá nhân của Việt Nam và các luật tương tự (như GDPR). Phần lớn có thể tự làm trong ứng dụng; các yêu cầu khác gửi qua email bên dưới.

Nếu chính sách này thay đổi, phiên bản mới sẽ được đăng tại trang này kèm ngày cập nhật.

Liên hệ: tiendatgiang.it@gmail.com

---

# Privacy Policy — Cội Nguồn

*Last updated: October 22, 2026*

Cội Nguồn is a family-tree app for Vietnamese clans on iOS (App Store) and Android (Google Play), developed by GLab. The app is free, has no ads, and we never sell or rent data.

## Data we store

- **Account.** When you sign in with Google or Apple, the app receives your display name, email and account identifier from that provider. With Apple you can hide your email. If you choose "Use without an account", the app only creates an anonymous identifier.
- **Family tree entered by you and your relatives.** Names, taboo / courtesy / posthumous names, gender, generation, branch, parent–spouse–child links, birth and death dates, death anniversaries, grave addresses, notes, portrait and grave photos. For living people it may also include phone numbers and addresses.
- **Clan information.** Clan name, ancestral hall address, the accounts that joined, each person's role, edit suggestions and invitations.
- **Crash reports.** When the app crashes, Firebase Crashlytics records technical details: device model, OS version, app version, crash logs and a random installation ID. Crash reports contain no family-tree content.
- **Abuse protection.** Firebase App Check uses Apple App Attest / DeviceCheck or Google Play Integrity to confirm that requests come from the genuine app.

The app does **not** use behavioural analytics, does **not** track you across other apps or websites, does **not** access advertising identifiers (IDFA, Android Advertising ID), and does **not** use location, microphone or contacts.

## How data is used

Only to provide the app's features: sign-in, storing and syncing the family tree between members, computing and reminding death anniversaries, inviting relatives, and fixing bugs.

## Who can see it

- Family trees are **private**: only accounts invited to the clan can see them.
- **Phone numbers and addresses** of living people are shown only to the Clan head, Branch editors and Members — not to Guests.
- Edit rights depend on role: Clan head, Branch editor (own branch), Member (suggests edits for the Clan head to approve).
- We share no data with any third party other than the infrastructure provider below.

## Where data is stored

Data is stored on **Google Firebase** (Authentication, Cloud Firestore, Crashlytics, App Check). Firestore is located in Singapore (`asia-southeast1`). Data is encrypted in transit (HTTPS/TLS) and at rest on Google's servers. The app keeps a cached copy of the tree on the device so it can be viewed offline.

## Device permissions

- **Camera, Photo library:** only when you choose to take or pick a portrait or grave photo. Photos are downscaled before saving.
- **Notifications:** death-anniversary reminders, scheduled on the device.

## Information about other people

A family tree contains information about relatives, including living people and children. Please only enter information that the person (or a child's parent or guardian) agrees to share within the clan. Anyone mentioned can ask the Clan head or us to correct or remove their information.

The app is not directed at children under 13 and does not knowingly collect data from children using it themselves.

## Retention and deletion

- **Delete account:** **Me → Delete account**. Your sign-in account and your membership in every clan are deleted immediately and cannot be restored; Apple / Google sign-in tokens are revoked. The family-tree entries you added stay with the clan because they are shared clan data. If you are the only member of a clan, that clan is deleted too.
- **Delete clan:** the Clan head can delete the whole clan (tree, photos, anniversaries, member list) under **Clan → Info**.
- **Remove a person:** the Clan head can delete a person's profile, photos and contact details.
- Data is kept until deleted as above. Crashlytics reports are deleted by Google after 90 days.
- Can't delete something in the app? Email us and we will handle it within 30 days.

## Your rights

You can access, correct and delete your data and withdraw consent at any time, under Vietnam's Decree 13/2023/ND-CP on personal data protection and similar laws (such as the GDPR). Most of this can be done in the app; send other requests to the email below.

If this policy changes, the new version will be posted on this page with a new date.

Contact: tiendatgiang.it@gmail.com
