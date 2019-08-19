# taro-react-apollo-hooks

`apollo-hooks` for `@tarojs/taro`

Fork from **react-apollo-hooks** (which already merged to [official React Apollo Hooks](https://www.npmjs.com/package/@apollo/react-hooks))

## tune-ment

- replace all `require("react")` to `require("@tarojs/taro")`

## usage

```javascript
import client from './apollo-client';
const QUERY = gql`
  {
    hi
  }
`;
// 为 useQuery 传入 client 参数即可
const { loading, error, data } = useQuery(QUERY, { client: overrideClient });
```
