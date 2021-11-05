---
title: Chat on MS Teams
script: >-
  javascript:(function(){
    let emails = [...document.querySelectorAll('.card-title-student')].map(st => /[0-9]{7}\@ucn.dk/i.exec(st.textContent)[0]);
    if(emails.length > 0){
      let topic = prompt('Name the chat', 'New chat');
      window.open(`https://teams.microsoft.com/l/chat/0/0?users=${emails.join(',')}&topicName=${topic}`);
    }else{
      alert('No emails selected.');
    }
  })();
---

This bookmarklet can be used for the site [UCN Student Management Portal](https://ucnstudents.ondni.com) to start a chat on MS Teams.
