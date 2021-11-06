---
title: Copy emails
script: >-
  javascript:(function(){
    let str = [...document.querySelectorAll('.card-title-student')].map(st => /[0-9]{7}\@ucn.dk/i.exec(st.textContent)[0]).join(';');
    prompt('Copy the text:', str);
  })();
---

This bookmarklet can be used for the site [UCN Student Management Portal](https://ucnstudents.ondni.com) to get a semicolon separated list of emails.
