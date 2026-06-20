1. Data fetching is implemented using the native `fetch` API together with **TanStack Query**, which provides efficient caching and network state management.
2. **Zustand** is a very common and lightweight state management solution. For a basic application like this, it looks like a perfectly suitable choice.
3. The search functionality takes the search text from the state and filters products using the `.filter()` method. The implementation is case-insensitive, which improves the user experience.
4. In some places, `useMemo` and `React.memo` could be applied to optimize rendering, especially since some props contain object values. Additionally, for more advanced networking requirements, **Axios** might be a better choice than the native `fetch` API.
