# hello-world
correspondences for the electronic production of loose ends literary works


loose - ends - interested in interactive coding for website platforms. 
looking to code a comment thread for experimental correspondences 

code 

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

for threaded comments 

"<script src="http://js-kit.com/comments.js"></script>"
