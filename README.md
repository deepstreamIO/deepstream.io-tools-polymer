# deepstream.io-tools-polymer

Polymer elements that makes it easy to sync with deepstream.

## Elements

### ds-record
```
<ds-record name="polymer_example/user" data="{{user}}" >
		<label>Name</label>
		<input type="text" value="{{user.name::input}}">
</ds-record>
```

### ds-list
```
<ds-list name="[[name]]" entries="{{todos}}" >
	<ul>
		<template is="dom-repeat" items="[[todos]]" as="recordId">
			<li>
				<span>[[recordId]]</span>
			</li>
		</template>
	</ul>
</ds-list>
```

## Behaviours

### DSRecordBehaviour
```
name: The record name to use. This can be changed dynamically and will update accordingly.
data: The object to use for two-way binding
```

### DSListBehaviour
```
name: The list name to use. This can be changed dynamically and will update accordingly.
entries: The array containing all record names within list
```
