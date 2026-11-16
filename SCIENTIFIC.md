# الأسس العلمية والمراجع — رفيق النجاح SEM

محرّك الحساب في البرنامج مستقل، ومبني على الأدبيات المنشورة في نمذجة المعادلات البنائية
بالمربعات الصغرى الجزئية. هذا الملف يوثّق المرجع الأساسي لكل طريقة يحسبها البرنامج.

## الخوارزمية الأساسية والمعايير
- **خوارزمية PLS-SEM:** Wold, H. (1982); Lohmöller, J.-B. (1989), *Latent Variable Path Modeling with Partial Least Squares*, Physica.
- **الممارسة والمعايير المرجعية:** Hair, J. F., Hult, G. T. M., Ringle, C. M., & Sarstedt, M. (2022), *A Primer on Partial Least Squares Structural Equation Modeling (PLS-SEM)*, 3rd ed., SAGE.
- **PLS المتسق (PLSc):** Dijkstra, T. K., & Henseler, J. (2015), *MIS Quarterly*, 39(2), 297–316.

## نموذج القياس
- **نسبة HTMT للصدق التمييزي:** Henseler, J., Ringle, C. M., & Sarstedt, M. (2015), *Journal of the Academy of Marketing Science*, 43(1), 115–135.
- **الموثوقية المركبة وrho_A:** Dijkstra & Henseler (2015); Jöreskog (1971).
- **المتغيرات من الرتبة العليا (عاكس-تكويني، مرحلتان):** Sarstedt, M., Hair, J. F., Cheah, J.-H., Becker, J.-M., & Ringle, C. M. (2019), *Australasian Marketing Journal*, 27(3), 197–211; Becker, Klein & Wetzels (2012), *LRP*, 45(5–6).

## النموذج البنائي
- **حجم الأثر f²:** Cohen, J. (1988), *Statistical Power Analysis for the Behavioral Sciences*, 2nd ed.
- **التعديل والوساطة المعدّلة:** Henseler, J., & Chin, W. W. (2010), *Structural Equation Modeling*, 17(1).
- **مؤشرات الملاءمة (SRMR):** Henseler et al. (2014), *ORM*; Hu & Bentler (1998).

## الاستدلال والتقييم التنبؤي
- **Bootstrapping:** Davison, A. C., & Hinkley, D. V. (1997), *Bootstrap Methods and Their Application*; Streukens & Leroi-Werelds (2016), *EMJ*, 34(6).
- **استدلال الملاءمة Bollen-Stine:** Bollen, K. A., & Stine, R. A. (1992), *Sociological Methods & Research*, 21(2).
- **Blindfolding وQ²:** Geisser, S. (1974), *Biometrika*, 61(1); Stone, M. (1974), *JRSS-B*, 36(2).
- **PLSpredict:** Shmueli, G., et al. (2016), *JBR*, 69(10); Shmueli et al. (2019), *EJM*, 53(11).
- **CVPAT:** Liengaard, B. D., et al. (2021), *Decision Sciences*, 52(2).

## المجموعات والتقسيم
- **تحليل متعدد المجموعات (MGA) وMICOM:** Henseler, J., Ringle, C. M., & Sarstedt, M. (2016), *International Marketing Review*, 33(3).
- **FIMIX-PLS:** Hahn, C., et al. (2002), *Schmalenbach Business Review*; Sarstedt, M., et al. (2011), *JFEC*.
- **PLS-POS:** Becker, J.-M., Rai, A., Ringle, C. M., & Völckner, F. (2013), *MIS Quarterly*, 37(3).

## التحليلات المتقدمة
- **IPMA — خريطة الأهمية والأداء:** Ringle, C. M., & Sarstedt, M. (2016), *Industrial Management & Data Systems*, 116(9).
- **NCA — تحليل الشروط الضرورية:** Dul, J. (2016), *Organizational Research Methods*, 19(1).
- **CTA-PLS — تحليل الرباعيات التأكيدي:** Gudergan, S. P., Ringle, C. M., Wende, S., & Will, A. (2008), *Journal of Business Research*, 61(12).
- **CB-SEM (الأرجحية العظمى):** Jöreskog, K. G. (1969), *Psychometrika*, 34(2).
- **نماذج PROCESS:** Hayes, A. F. (2022), *Introduction to Mediation, Moderation, and Conditional Process Analysis*, 3rd ed., Guilford.

## التحقق من الموثوقية
طُوبقت مخرجات البرنامج مع برنامج **SmartPLS 4** ومكتبة **seminr** (في لغة R) على النماذج نفسها
والبيانات نفسها، جدولاً جدولاً، إلى ثلاث منازل عشرية: معاملات المسار، والأوزان، والتحميلات،
وR²، وf²، وHTMT، وQ²، وSRMR، وBootstrapping، وMGA، وMICOM، والميول البسيطة.

واجتاز البرنامج قبل كل إطلاق فحصاً آلياً شاملاً يشغّل جميع التحليلات على النماذج المرجعية
الأربعة المرفقة؛ تفاصيل آخر تشغيل في [docs/pre-release-diagnostics.md](docs/pre-release-diagnostics.md).
