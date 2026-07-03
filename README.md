# אתר הראל מתכת בע״מ — harel-metal.com

אתר סטטי (עמוד אחד) בעברית (RTL), ללא וורדפרס וללא בסיס נתונים.
מתארח בחינם ב־**GitHub Pages**.

## מבנה הקבצים
```
index.html          — כל תוכן העמוד + העיצוב (CSS מוטמע)
images/             — תמונות (לוגו, גלריית מוצרים, תמונת "אודות")
pdfs/               — עלון החברה + תעודות ISO 9001 (עברית/אנגלית)
robots.txt          — הנחיות למנועי חיפוש
sitemap.xml         — מפת אתר לגוגל
CNAME               — הדומיין המותאם (harel-metal.com)
.nojekyll           — אומר ל־GitHub Pages להגיש את הקבצים כמו שהם
```

## איך לערוך את האתר
כל הטקסטים נמצאים ב־`index.html`. פותחים את הקובץ, מחפשים את הטקסט לעריכה,
משנים, שומרים ו־commit — האתר מתעדכן אוטומטית תוך דקה.
מחליפים תמונה? מעלים קובץ בשם זהה לתיקיית `images/`.

## פרסום ל־GitHub Pages (פעם אחת)
1. צרו חשבון ב־https://github.com והתקינו/היכנסו.
2. צרו repository חדש (למשל בשם `harel-metal`).
3. העלו את כל הקבצים מתיקייה זו ל־repository:
   - דרך הדפדפן: **Add file → Upload files** וגררו את כל הקבצים (כולל התיקיות images/ ו־pdfs/).
   - או דרך git:
     ```bash
     cd site
     git init
     git add .
     git commit -m "Harel Metal static site"
     git branch -M main
     git remote add origin https://github.com/<שם-המשתמש>/harel-metal.git
     git push -u origin main
     ```
4. ב־repository: **Settings → Pages → Source: Deploy from a branch → main / (root) → Save**.
5. תוך דקה-שתיים האתר יעלה בכתובת `https://<שם-המשתמש>.github.io/harel-metal/`.

## חיבור הדומיין harel-metal.com
1. ב־**Settings → Pages → Custom domain** הקלידו `harel-metal.com` ו־Save
   (קובץ ה־CNAME כבר קיים ב־repo).
2. אצל רשם הדומיין (היכן שקניתם את harel-metal.com — כנראה Bluehost) עדכנו DNS:
   - רשומות **A** ל־apex (`@`) לכתובות של GitHub:
     ```
     185.199.108.153
     185.199.109.153
     185.199.110.153
     185.199.111.153
     ```
   - רשומת **CNAME** ל־`www` → `<שם-המשתמש>.github.io`
3. חזרו ל־Settings → Pages וסמנו **Enforce HTTPS** (יופיע אחרי שה־DNS מתעדכן, ~15 דק׳–שעה).

## הוספת שותף/ה לניהול
ב־repository: **Settings → Collaborators → Add people**.

## אחרי שהאתר עובד
- הוסיפו את האתר ל־**Google Search Console** (https://search.google.com/search-console),
  אמתו בעלות ושלחו את `sitemap.xml`.
- רק אחרי אימות שהאתר החדש עובד — אפשר לבטל את אחסון ה־WordPress ב־Bluehost
  (חשוב לשמור את רישום הדומיין!).

## מספרי קשר באתר
- טלפון: 03-9642913
- וואטסאפ: 054-803-0412 (972548030412)
- כתובת: רחוב פלוטיצקי 8, ראשון לציון
