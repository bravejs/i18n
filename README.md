# i18n

## Interface
```ts
interface Messages {
    [K: string]: any;
}

interface Values {
    [K: string]: any;
}

export interface Options {
    locale: string;
    fallbackLocale: string;
    messages: Messages;
}

declare class I18n {
    locale: string;
    
    constructor(options: Options);
    
    t(key: string, values?: Values): any;
    
    setLocale(locale: string): void;
    
    destroy(): void;
}
```
