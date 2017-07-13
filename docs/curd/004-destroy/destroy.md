# destroy
> DELETE /posts/1

## controller:
```rb
def destroy
  post = Post.find params[:id]
  if post.destroy
    redirect_to posts_path, flash: { notice: 'Your post has been removed.' }
  else
    redirect_to posts_path, flash: { error: 'We were unable to remove that post.' }
  end
end
```

## views:
```rb
<%= link_to 'delete', post_path(@post), method: :delete %>
```
