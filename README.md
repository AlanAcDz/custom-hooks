# Notes

This repo contains diverse React custom hooks and helpers, so that I don't have to rewrite them ;)

## Hooks

### useCounter

This hook works like a simple counter. It receives a default value, and returns an object with the current value alongside an increment, decrement & reset functions
Example:
```
    const { counter, increment, decrement, reset } = useCounter(10);
```

### useFetch

This hook helps fetching data from an API endpoint. It receives the endpoint URL, and returns an object with the data, loading state & errors
Example:
```
    const { data, loading, error } = useFetch(url);
```

### useForm

This hooks helps managing forms. It receives an object with all the form fields, and returns an array with the form values alongside a handleInputChange & reset functions
Example:
```
    const initialForm = {
        ...formFields
    };
    const [ values, handleInputChange, reset ] = useForm(initialForm);
```