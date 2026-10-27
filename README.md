# Seha Referrals App for Case Coordinators

**By Dr.Fahad Aldawood**

Windows application with three Seha School Screening workflows: verified referral lookup, auditor approval of pending reports, and incremental Excel export of completed referral-list data. Includes Arabic/English controls, full PHC/role names, a custom icon and GitHub updates.

## Download and start

1. Open [the latest release](https://github.com/DrFnan194/Seha-Referrals-App-For-Case-Coordinators/releases/latest).
2. Download **SehaReferral-Windows-x64.zip** and extract all files into a permanent user-writable folder.
3. Run **SehaReferralApp.exe**, choose the workflow, and sign in normally through Seha/Nafath with your own account.
4. Choose an authorized PHC for a single-center action, or use the bulk action and review its PHC checkboxes before starting.

## Version 1.4.4

- Bulk approval and completed-data export can visit the selected authorized PHCs automatically.
- PHC checkboxes, Select all, Clear all and a selected count let users exclude unwanted centers. Empty selections cannot start.
- Opening a PHC allows two attempts, with a fresh portal reload before the second attempt. Two failures skip that center and appear in the final summary. Processing failures or uncertain approval outcomes stop the run without replaying a write.
- Longer navigation/list waits accommodate slow service responses. Final summaries distinguish completed, skipped, excluded and not-reached centers.
- Completed exports include the referral-list columns, PHC and pull timestamp. The app remembers the selected workbook and appends new scoped report identities only. Existing rows and their timestamps are retained.
- Lookup uses the same identifier previously labelled Student ID, now labelled Referral ID. Student, screening and selected-PHC identity must verify before the report is presented as matched.

## الاستخدام بالعربية

نزّل الحزمة من صفحة الإصدارات، واستخرج جميع ملفاتها، ثم شغّل **SehaReferralApp.exe** واختر الدور:

- **مدخل بيانات متابعة الإحالات:** اختيار المركز وفتح القائمة ثم البحث برقم الإحالة والتحقق من هوية الطالب والفحص.
- **مدقق متابعة الإحالات:** اعتماد تقارير «تحت التدقيق» للمركز المختار، أو للمراكز المحددة في قائمة مربعات الاختيار.
- **سحب تفاصيل البيانات المكتملة:** اختيار ملف Excel وإغلاقه في Excel، ثم سحب بيانات «مكتمل» للمركز المختار أو للمراكز المحددة، مع إضافة غير الموجود فقط.

في العمليات الجماعية أزل علامة الاختيار عن أي مركز غير مطلوب، وراجع عدد المراكز ثم اضغط **بدء العملية للمراكز المحددة**. المراكز المستبعدة باختيارك تختلف عن المراكز المتخطاة بعد فشل الفتح. «مراكز لم يصل إليها التشغيل» تعني توقف العملية قبل زيارتها. وعدّاد التقارير المكتملة عند إعادة التحقق يخص الدفعة الحالية، وليس السجل التاريخي كله.

## Updates

From version 1.1.0, the app checks public GitHub Releases for newer stable versions. Finish current work and return to the list, then choose **التحقق من التحديثات / Check for updates** and **تنزيل التحديث وإعادة التشغيل / Download and restart**. Earlier builds require one manual installation.

The updater checks GitHub's SHA-256 digest, backs up replaced application files and preserves the separate Seha browser profile, language and workbook preference. Members do not need a GitHub account for public downloads or update checks.

Each member uses their own normal Seha permissions. Data entry does not save clinical form changes automatically; the separate auditor workflow submits only the approvals explicitly started by the user. Seha remains the authoritative system. Excel links are temporarily disabled.

This repository hosts release downloads. The complete application source is attached to each release separately from GitHub's automatic tag archives. No patient workbooks, clinical screenshots, credentials, browser profiles or private validation checkpoints belong in releases or repository commits.