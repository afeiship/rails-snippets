# update
> PATCH/PUT /models/1

## snippets:
```rb
  def update
    if @item.update(allow_params)
      redirect_to @item, notice: 'Model was successfully updated.'
    else
      render :edit
    end
  end
```
