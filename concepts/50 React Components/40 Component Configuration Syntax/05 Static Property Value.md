    <!-- tab: Function component -->
    import Button from 'devextreme-react/button';

    export default function App() {
        return (
            <Button
                disabled={false}
                width={50}
                text="Click me"
            />
        );
    }
    
    <!-- tab: Class component -->
    import Button from 'devextreme-react/button';

    class App extends React.Component {
        render() {
            return (
                <Button
                    disabled={false}
                    width={50}
                    text="Click me"
                />
            );
        }
    }