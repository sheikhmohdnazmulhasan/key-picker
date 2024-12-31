# key-picker

A utility to pick specific keys from an object, useful for filtering valid query strings.

## Installation

You can install `key-picker` using npm:

```bash
npm install key-picker
```

## Usage

Here's how you can use the `pick` function from `key-picker`:

```typescript
import pick from "key-picker";

const obj = {
  name: "John Doe",
  age: 30,
  email: "john@example.com",
  address: "123 Main St",
};

const selectedKeys = ["name", "email"];
const result = pick(obj, selectedKeys);

console.log(result);
// Output: { name: 'John Doe', email: 'john@example.com' }
```

## API

```typescript
pick<T extends Record<string, unknown>, K extends keyof T>(obj: T, keys: K[]): Partial<T>
```

## TypeScript Support

`key-picker` is written in TypeScript and includes type definitions. It provides full type inference for better development experience.

## Use Cases

- Filtering query parameters for API requests
- Extracting specific properties from large objects
- Creating subsets of configuration objects

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Author

Sheikh Mohammad Nazmul H. - [GitHub](https://github.com/sheikhmohdnazmulhasan)

## Issues

If you encounter any issues or have feature requests, please file them in the [issues section](https://github.com/sheikhmohdnazmulhasan/pick-me/issues).
