# useState() Hook

### What is a Hook? ? 
Hooks are a type of function that allows you to "hook onto" React capabilities. UseState, for example, is a Hook that adds React state to function components. Other Hooks will be covered later.

### When would I use a Hook?
You used to have to change a function component to a class if you realized you needed to add some state to it. You can now use a Hook within a function component that already exists.

### What does calling useState do?
The concept of a "state variable" is introduced. Our variable is called count, but it might be anything other, such as banana. This is a new way to access the same features. In a class, the state provides — make advantage of it. State is a novel approach to keep some variables "alive" between function calls. When a function exits, variables usually "disappear," however state variables are preserved in React.

### What do we pass to useState as an argument? 
The starting state is the only input to the useState() Hook. The state, unlike classes, does not have to be an object. If all we need is a number or a string, we can keep it. We merely want a number for how many times the user clicked in our example, so set our variable's initial state to 0. (We would call useState() twice if we wanted to store two different values in state.)

### What does useState return?
It returns a two sets of values: the current state and an update function. This is why const [count, setCount] = useState is written (). This is a comparable situation. The only difference between state.count and this.setState in a class is that you get them in a pair. We'll go over the syntax again if you're unfamiliar with it.

### Hooks Api and Reference

Hooks are a new addition in React they let you use state and other React features without writing a class.

### below are built-in Hooks in React.

### Basic Hooks:
useState
useEffect
useContext

### Additional Hooks:
useReducer
useCallback
useMemo
useRef
useImperativeHandle
useLayoutEffect
useDebugValue
useDeferredValue
useTransition
useId
