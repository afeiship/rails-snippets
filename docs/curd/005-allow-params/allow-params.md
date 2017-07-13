# allow-params
!> Never trust parameters from the scary internet, only allow the white list through.


## snippets:
```rb
private
  def allow_params
    params.require(:model).permit(:field1, :field2)
  end
```
