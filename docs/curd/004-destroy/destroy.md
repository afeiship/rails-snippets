# destroy
> DELETE /models/1

## snippets:
```rb
def destroy
  set_item
  @post.destroy
  redirect_to items_url, notice: 'Model was successfully destroyed.'
end
```
