# VOLVOX GAMES UNITY NAMING CONVENTIONS

- <a href="#examplecs">Example.cs</a>
- <a href="method">Methods</a>
- <a href="typedefinitions">Type Definitions</a>

## Example.cs

```cs
// CONSTANTS -------------------------------------------------------------------------------

public const int PUBLIC_COMPILE_TIME_CONSTANT = 0;
public static readonly int PUBLIC_RUNTIME_CONSTANT;

protected const int PROTECTED_COMPILE_TIME_CONSTANT = 0;
protected static readonly int PROTECTED_RUNTIME_CONSTANT;

private const int PRIVATE_COMPILE_TIME_CONSTANT = 0;
private static readonly int PRIVATE_RUNTIME_CONSTANT;


// EVENTS -----------------------------------------------------------------------------------

public static event Action<> OnStaticGenericEvent;
public static event Action OnStaticEvent;

public event Action<> OnGenericEvent;
public event Action OnEvent;


// STATIC FIELDS ----------------------------------------------------------------------------
// STATIC VALUE FIELDS ARE NOT ALLOWED!

public static int PublicStaticField;

protected static int ProtectedStaticField;

private static int ms_PrivateStaticField;


// FIELDS -----------------------------------------------------------------------------------

[SerializeField] private int _serializedField;

protected int protectedField;

private int m_PrivateField;


// MONOBEHAVIOUR CALLBACKS ------------------------------------------------------------------

private void Awake()
{

}

private void Start()
{

}

private void OnEnable()
{

}

private void OnDisable()
{

}

private void OnDestroy()
{

}

private void Update()
{

}

private void FixedUpdate()
{

}

private void LateUpdate()
{

}


// EVENT LISTENERS -----------------------------------------------------------------------------------

private void OnEventRaised()
{

}


// PUBLIC METHODS -----------------------------------------------------------------------------------

public void PublicMethod()
{

}


// PROTECTED METHODS -----------------------------------------------------------------------------------

protected void ProtectedMethod()
{

}


// PRIVATE METHODS -----------------------------------------------------------------------------------

private void PrivateMethod()
{

}


// PUBLIC STATIC METHODS -----------------------------------------------------------------------------------

public static void PublicStaticMethod()
{

}


// PROTECTED STATIC METHODS -----------------------------------------------------------------------------------

protected static void ProtectedStaticMethod()
{

}


// PRIVATE STATIC METHODS -----------------------------------------------------------------------------------

private static void PrivateStaticMethod()
{

}
```

## Methods {#methods}

```cs
private void Method(int number, string text)
{
    const int localConstant = 0;

    int localVariable;
}

public int GetInt()
{
    return 0;
}

public void SetInt(int value)
{
    ms_Value = value;
}
```

## Type Definitions {#type-definitions}

```cs
public enum Direction
{
    North,
    South,
    East,
    West
}
```
