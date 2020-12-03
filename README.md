# hello-world
correspondences for the electronic production of loose ends literary works


loose - ends - interested in interactive coding for website platforms. 

threaded comments research for experimental correspondences 

test 01 - leave a comment

<div id="respond">

  <h3>Leave a Comment</h3>

  <form action="post_comment.php" method="post" id="commentform">

    <label for="comment_author" class="required">Your name</label>
    <input type="text" name="comment_author" id="comment_author" value="" tabindex="1" required="required">

    <label for="email" class="required">Your email;</label>
    <input type="email" name="email" id="email" value="" tabindex="2" required="required">

    <label for="comment" class="required">Your message</label>
    <textarea name="comment" id="comment" rows="10" tabindex="4"  required="required"></textarea>

    <-- comment_post_ID value hard-coded as 1 -->
    <input type="hidden" name="comment_post_ID" value="1" id="comment_post_ID" />
    <input name="submit" type="submit" value="Submit comment" />

  </form>

</div>

#respond {
  margin-top: 40px;
}

#respond input[type='text'],
#respond input[type='email'], 
#respond textarea {
  margin-bottom: 10px;
  display: block;
  width: 100%;

  border: 1px solid rgba(0, 0, 0, 0.1);
  -webkit-border-radius: 5px;
  -moz-border-radius: 5px;
  -o-border-radius: 5px;
  -ms-border-radius: 5px;
  -khtml-border-radius: 5px;
  border-radius: 5px;

  line-height: 1.4em;
}



text 02 threaded comment 

"<script src="http://js-kit.com/comments.js"></script>"



test 03 threaded comment

-> {'text': "parent", id: "parent"}
      -> {'text': "child1", parentid= "parent", id: "child1"} // reply to the parent
      -> {'text': "child1.1", parentid= "parent", id: "child2"} // reply to the parent
      -> {'text': "child2", parentid: "child1" id: "child3"} // reply to the child1
      
          "parent": {
        'text': "parent",
        id: "parent",
        children: {
            child1: {
                text: "child1",
                parentid = "parent",
                id: "child1",
                children: {
                    child3: {
                        text: "child2",
                        parentid: "child1"
                        id: "child3"
                    }
                }
            },
            child2: {...}
        }
    }
}
      
      
      
      
      test 04 threaded comment
      
      var Worker = require('webworker-threads').Worker;
// var w = new Worker('worker.js'); // Standard API

// You may also pass in a function:
var worker = new Worker(function(){
  postMessage("I'm working before postMessage('ali').");
  this.onmessage = function(event) {
    postMessage('Hi ' + event.data);
    self.close();
  };
});
worker.onmessage = function(event) {
  console.log("Worker said : " + event.data);
};
worker.postMessage('ali');



test 05 


/*     
   The baseline. This will be applied to any browser that does not
   support calc, and any browser that is smaller than 800px wide 
*/
.comments-list, 
.comment { 
    width: 100%; 
}

.comments-section .children {
    margin-left: 5%;
    padding-left: 0;
    width: 95%;
}

/* 
  For browser over 800px wide (50em = 800px), threaded comment blocks are
  indented by a specific unit -- not percentages.
  Note that our root font size is 10px, so 1rem = 10px and 7rem = 70px. 
*/
@media all and (min-width: 50em) {
    .comments-section .children {       
    /* Why the use of calc for margin-left? 
       Because browsers that don't support calc will be served 
       up the mobile styling, which is percentage based.  */
    margin-left: calc( 7rem );
    margin-left: -moz-calc( 7rem );
    margin-left: -webkit-calc( 7rem );

    width: calc(100% - 7rem);
    width: -moz-calc(100% - 7rem);
    width: -webkit-calc(100% - 7rem);
    }
}



test 06

<script src="https://cdn.fastcomments.com/js/embed.min.js"></script>
<div id="fastcomments-widget"></div>
<script>
    window.FastCommentsUI(document.getElementById('fastcomments-widget'), {
        tenantId: 'iF4LUmi9a'
    });
</script>



"<script src="http://js-kit.com/comments.js"></script>"
<div id="js-kit.com/comments.js"></div>
<script>
   window.jscomments(document.getElementById('jscomments-js'), {
        tenantId: 'iF4LUmi9a'
    });
</script>



test 07


#comments { display: block; }

#comments .cmmnt, ul .cmmnt, ul ul .cmmnt { display: block; position: relative; padding-left: 65px; border-top: 1px solid #ddd; }

#comments .cmmnt .avatar  { position: absolute; top: 8px; left: 0; }
#comments .cmmnt .avatar img { 
  -webkit-border-radius: 3px; 
  -moz-border-radius: 3px; 
  border-radius: 3px; 
  -webkit-box-shadow: 1px 1px 2px rgba(0,0,0,0.44);
  -moz-box-shadow: 1px 1px 2px rgba(0,0,0,0.44);
  box-shadow: 1px 1px 2px rgba(0,0,0,0.44);
  -webkit-transition: all 0.4s linear;
  -moz-transition: all 0.4s linear;
  -ms-transition: all 0.4s linear;
  -o-transition: all 0.4s linear;
  transition: all 0.4s linear;
}

#comments .cmmnt .avatar a:hover img { opacity: 0.77; }

#comments .cmmnt .cmmnt-content { padding: 0px 3px; padding-bottom: 12px; padding-top: 8px; }
#comments .cmmnt .cmmnt-content header { font-size: 1.3em; display: block; margin-bottom: 8px; }
#comments .cmmnt .cmmnt-content header .pubdate { color: #777; }
#comments .cmmnt .cmmnt-content header .userlink { font-weight: bold; } 
#comments .cmmnt .replies { margin-bottom: 7px; }

test 08

<html lang="en">
<head>
  <meta charset="UTF-8" />
  <title>Document</title>
</head>
<body>
  <header class="header">
    <div class="container">
      <div class="row">
        <div class="col-xs-12">
          <h1>threadly</h1>
        </div>
      </div>
    </div>
  </header>
  <div class="main">
    <div class="container">
      <div class="row">
        <form action="" class="form">
          <div class="col-xs-8 col-md-10">
            <input type="text" id="comment" placeholder="say something" />
          </div>
          <div class="col-xs-4 col-md-2">
            <button type="submit" class="btn">post</button>
          </div>
        </form>
      </div>
      <ul class="comments" id="comments">
        <!-- <li>My first comment: Hello world!</li> -->
      </ul>
    </div>
  </div>
</body>
</html>






