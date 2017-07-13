# create
> POST /posts

## snippets:
```rb
  def create
    @item = Model.new(allow-params)
    if @item.save
      redirect_to @item, notice: 'Item was successfully created.'
    else
      render :new
    end
  end
```
