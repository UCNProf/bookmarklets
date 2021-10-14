---
title: Copy URL as Markdown
script: >-
  javascript:(function(){
    let getSelectionText = () => {
      let text = '';
      if (window.getSelection){
        text = window.getSelection().toString();
      }
      return text;
    };
    let clip = getSelectionText();var texttocopy = ((clip)?clip+' ':'')+`[${document.title}](${window.location})`;
    prompt('Copy the text:', texttocopy);
  })();
---

This bookmarklet can be used for copying URL, title and selected content as Markdown.
