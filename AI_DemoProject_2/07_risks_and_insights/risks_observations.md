# Risks and Observations – ToDo Application

## Risks
- **Incomplete requirements:** Missing details may lead to gaps in test coverage.
- **Environment instability:** Demo app may not always be available, blocking test execution.
- **Data consistency issues:** Tasks created in UI may not always match API responses.
- **Usability risks:** Error messages may be unclear, reducing user satisfaction.

## Observations
- Double-click issue shows lack of debounce in UI.
- Error messages are technical (e.g., "400 Bad Request") instead of user-friendly.
- Filtering works correctly but reset button is not intuitive.
- Accessibility checks revealed missing focus indicators on some interactive elements.

## Recommendations
- Improve error messages to be understandable for end users.
- Add debounce or disable buttons to prevent duplicate actions.
- Ensure consistency between UI and API responses.
- Enhance accessibility by adding visible focus indicators and improving contrast.
