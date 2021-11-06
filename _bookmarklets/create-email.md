---
title: Create email
script: >-
  javascript:(function(){
    let emails = userResults.map(st => `"${st.Value.FirstLine}" <${st.Value.Email}>`);
    if(emails.length > 0){
      window.open(`https://outlook.office.com/mail/deeplink/compose?to=${emails.join(',')}`);
    }else{
      alert('No emails selected.');
    }
  })();
---

This bookmarklet can be used for the site [UCN Student Management Portal](https://ucnstudents.ondni.com) to create an email in MS Office 365 to the selected students.
