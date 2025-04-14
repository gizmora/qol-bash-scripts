# Copy build files to Clasp folder (Google App Script)

```bash
cp ./dist/<project-folder>/main.*.js ./clasp/<clasp-folder>/main.js.html


echo "<script type=\"module\">" > temp
cat ./clasp/app/main.js.html >> temp
echo "</script>" >> temp
mv temp ./clasp/app/main.js.html


cp ./dist/<project-folder>/styles.*.css ./clasp/<clasp-folder>/styles.css.html

echo "<style>" > temp
cat ./clasp/<clasp-folder>/styles.css.html >> temp
echo "</style>" >> temp
mv temp ./clasp/<clasp-folder>/styles.css.html
```
