# YUUKIToriyama/yorimichi-images

[Cocon/yorimichi](https://github.com/Cocon/yorimichi)で表示するルートデータをホストします。

```typescript
export interface DateTime {
	year: number | string;
	month: number | string;
	day: number | string;
	time?: string;
}
export interface Location {
	longitude: number;
	latitude: number;
}
export interface Place {
	name: string;
	description: string;
	image?: string[];
	location: Location;
}
export interface RouteData {
	title: string;
	description?: string;
	roadNames?: string[];
	date: DateTime;
	updateDate?: DateTime;
	route: Place[];
}
```
