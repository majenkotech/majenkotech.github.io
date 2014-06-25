// $Id: script.js,v 1.1.2.3 2008/12/28 02:44:37 eric3 Exp $

// Adds drop-down menu functionality to IE6.
// Source: http://www.alistapart.com/articles/horizdropdowns/
menuOver=function(navRoot) {
  for (i=0; i<navRoot.childNodes.length; i++) {
    node = navRoot.childNodes[i];
    if (node.nodeName=="LI") {
      node.onmouseover=function() {
        //this.className+=" over";
        for (j=0; j<this.childNodes.length; j++) {
          childnode = this.childNodes[j];
          if (childnode.nodeName=="A") {
            childnode.className+=" over";
          }
          if (childnode.nodeName=="UL") {
            childnode.className+=" show";
          }
        }
      }
      node.onmouseout=function() {
        //this.className=this.className.replace(" over", "");
        for (j=0; j<this.childNodes.length; j++) {
          childnode = this.childNodes[j];
          if (childnode.nodeName=="A") {
            childnode.className=childnode.className.replace(" over", "");
          }
          if (childnode.nodeName=="UL") {
            childnode.className=childnode.className.replace(" show", "");
          }
        }
      }
    }
  }
}
startList=function() {
  if (document.getElementById) {
    menuOver(document.getElementById("primary-links"));
    menuOver(document.getElementById("tertiary-links"));
  }
}
window.onload=startList;
