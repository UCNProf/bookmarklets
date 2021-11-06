---
title: Copy emails
script: >-
  javascript:(function(){
    let emails = userResults.map(st => st.Value.Email).join(';');
    prompt('Copy the text:', emails);
  })();
---

This bookmarklet can be used for the site [UCN Student Management Portal](https://ucnstudents.ondni.com) to get a semicolon separated list of emails of the selected students.
