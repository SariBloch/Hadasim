# Hadasim
home task
RR:
server:
*ההתממשקות לטכנולוגית איכוני טלפונים תהיה בצד השרת
כאשר נקבל מהקליינט הודעה עם נ.צ ותאריך נוכל להשתמש בטכנולוגיה זו ולאתר את כל האנשים ששהו בקרבת מקום
הפונקציה תחשב את תאריך ההחלמה לפי תאריך החשיפה לנגיף שקיבלה מהקליינט ותחזיר אוביקט עם השדות:
תאריך חשיפה לנגיף, מיקום, תאריך החלמה , מערך אנשים שיש לעדכן

*לא תינתן אפשרות לשלוח הודעה עם שדות חסרים ולכן סטטוס 400 לא יהווה שגיאה של שדה חסר
אלא של שדה לא תקיו

*בכל קריאה לשרת יוחזר לקליינט אוביקט עם הנתונים המעודכנים + סטטוס הצלחה/כישלון

UI:
*בלחיצה על כפתור "צור בידוד" נשלחת בקשה אל השרת ולא אל הקליינט כפי שצוין באיפיון

*כפתור הצור בידוד לא יהיה מאופשר כל עוד לא נבחרו מיקום ותאריך

*ביציאה מתיבת הקלט של החיפוש יופיע PlaceHolder 
עם הכיתוב "זהו שדה חובה" 

*בלחיצה על צור בידוד, במידה וחזר מהשרת סטטוס 201 המשתמש ינותב לטופס שיציג את הנתונים שחזרו מהשרת
תאריך חשיפה, תאריך החלמה, מיקום, רשימת אנשים לעדכון

*בקבלת סטטוס 400 תופיע הודעת שגיאה והמשתמש יוחזר אוטומטית אל הטופס הקודם לבחירת הנתונים מחדש



Testing:

*בדיקת תקינות הקלט בצד שרת של שדות האוביקט שמתקבל

*בדיקה של מערך האנשים שחוזר לי מטכנולוגית איכוני הטלפונים של כלל אוכלוסיית ישראל

*בדיקת המיקום שנשלח מהקליינט (מקום ישוב הגיוני)

*ניסיון ובדיקות ע"י הכלי פוסטמן של קבלת נתונים נכונים למקרים השונים



User manual:
*יש להריץ את צד השרת וצד הלקוח במקביל:
פתיחת פרויקט הסרבר בויזואל סטודיו והרצה בכפתור המרכזי שבסרגל הכלים העליון(עם ציור של משולש ירוק)
פתיחת פרויקט הקליינט בויזואל סטודיו קוד והרצה ע"י הרצת הפקודה הבאה בטרמינל:
npm run start

*יש להדליק/להרים/להריץ את הסרביסים של הטכנולוגיות הנדרשות ולראות שאכן אנחנו מקבלים נתונים
*
