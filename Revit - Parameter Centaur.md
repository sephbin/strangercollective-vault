Revit parameters don't have a decent way to limit their input with conditions.
For example: _on a project we might want to limit the pattern for room numbers to be: "BLD-L[0-9]+-[0-9]{3}". Users can enter "BLDG_L0-04" without any function that flags warnings or corrects the result._

I am unaware of a vanilla way to limit these without running through the model and checking them after the fact.

Is it possible to create a plugin that validates the data entry as an object is edited? I was thinking maybe we can replace the vanilla parameter editor with a plugin parameter editor. This would allows us to create extra features like dropdowns and allow data entry validation. BUT, the parameter editor isn't the only place parameters can be set.

Instead, is it possible to add a function to the event 