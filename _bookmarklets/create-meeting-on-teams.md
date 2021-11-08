---
title: Create a MS Teams Meeting
script: >-
  javascript:(function(){
    let emails = selectedusers.map(id => userResults.find(st => st.Key == id )).map(st => st.Value.Email);
    if(emails.length > 0){
      window.open(`https://teams.microsoft.com/l/meeting/new?attendees=${emails.join(',')}`);
    }else{
      alert('No emails selected.');
    }
  })();
---

This bookmarklet can be used for the site [UCN Student Management Portal](https://ucnstudents.ondni.com) to create a meeting on MS Teams with the selected students.
