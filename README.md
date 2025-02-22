# Emotion + React Native Snippets

A collection of VSCode snippets for styling React Native components with Emotion.

## Installation

1. Open VSCode
2. Press `Cmd+Shift+P` (Mac) or `Ctrl+Shift+P` (Windows/Linux)
3. psate the following command `ext install rn-emotion-snippets` and press enter.

Alternatively you can open extensions panel and search for `Reactnative emotion snippets`.

## Supported Languages

These snippets are designed to work with:
- JavaScript (.js)
- TypeScript (.ts)
- React (.jsx)
- React TypeScript (.tsx)

## Available Snippets

Our snippets follow a consistent naming convention:
- `etc-componentName`: Stands for "Emotion Theme Component" - Creates a component with theme support
- `et-componentName`: Stands for "Emotion Component" - Creates a basic component without theme

### Snippet Reference Table

| Prefix | Component | Description |
|--------|-----------|-------------|
| `etc-view`, `etcview` | View | Creates a styled View component |
| `et-view`, `etview` | View | Creates a basic styled View |
| `etc-text`, `etctext` | Text | Creates a styled Text component |
| `et-text`, `ettext` | Text | Creates a basic styled Text |
| `etc-touch`, `etctouch` | TouchableOpacity | Creates a styled TouchableOpacity |
| `et-touch`, `ettouch` | TouchableOpacity | Creates a basic styled TouchableOpacity |
| `etc-image`, `etcimage` | Image | Creates a styled Image component |
| `et-image`, `etimage` | Image | Creates a basic styled Image |
| `etc-scroll`, `etcscroll` | ScrollView | Creates a styled ScrollView |
| `et-scroll`, `etscroll` | ScrollView | Creates a basic styled ScrollView |
| `etc-input`, `etcinput` | TextInput | Creates a styled TextInput |
| `et-input`, `etinput` | TextInput | Creates a basic styled TextInput |
| `etc-list`, `etclist` | FlatList | Creates a styled FlatList |
| `et-list`, `etlist` | FlatList | Creates a basic styled FlatList |
| `etc-safe`, `etcsafe` | SafeAreaView | Creates a styled SafeAreaView |
| `et-safe`, `etsafe` | SafeAreaView | Creates a basic styled SafeAreaView |
| `etc-button`, `etcbutton` | Button (Pressable) | Creates a styled Button component |
| `et-button`, `etbutton` | Button (Pressable) | Creates a basic styled Button |

### Usage Example

```jsx
// With theme support
const StyledView = styled.View(({theme}) => ({
    flex: 1,
    backgroundColor: theme.colors.background
}));

// Without theme support
const BasicView = styled.View({
    flex: 1,
    backgroundColor: '#ffffff'
});
```

### Notes

- Theme-supported components (`etc-`) expect a theme object to be available through React's context
- All components automatically use the current filename as the default component name
- Basic components (`et-`) use hardcoded values instead of theme references
- Button components use Pressable as the base component for better flexibility