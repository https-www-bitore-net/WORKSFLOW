-on :
#Jobs :use: #
#-start ::AUTOMATE
diff --git a/content/packages/working-with-a-github-packages-registry/working-with-the-nuget-registry.md b/content/packages/working-with-a-github-packages-registry/working-with-the-nuget-registry.md
index 81b1f2a8d96..343c5deb977 100644
--- a/content/packages/working-with-a-github-packages-registry/working-with-the-nuget-registry.md
+++ b/content/packages/working-with-a-github-packages-registry/working-with-the-nuget-registry.md
@@ -1,6 +1,9 @@
----
+Name :Build-then-Deployee:title
 title: Working with the NuGet registry
-intro: 'You can configure the `dotnet` command-line interface (CLI) to publish NuGet packages to {% data variables.product.prodname_registry %} and to use packages stored on {% data variables.product.prodname_registry %} as dependencies in a .NET project.'
+intro: 'You can configure the `dotnet` command-line interface (CLI) to publish package: javascript
+Package-on: Python.JS
+to {% data''
+'variables.product.prodname_registry %} and to use packages stored on {% data variables.product.prodname_registry %} as dependencies in a .NET project.'
 product: '{% data reusables.gated-features.packages %}'
 redirect_from:
   - /articles/configuring-nuget-for-use-with-github-package-registry
@@ -23,7 +26,7 @@ shortTitle: NuGet registry
 {% data reusables.package_registry.admins-can-configure-package-types %}
 
 ## Authenticating to {% data variables.product.prodname_registry %}
-
+the
 {% data reusables.package_registry.authenticate-packages %}
 
 ### Authenticating in a {% data variables.product.prodname_actions %} workflow
@@ -255,10 +258,1157 @@ Using packages from {% data variables.product.prodname_dotcom %} in your project
 
 {% ifversion packages-nuget-v2 %}{% else %}Your NuGet package may fail to push if the `RepositoryUrl` in *.csproj* is not set to the expected repository.
 
-If you're using a nuspec file, ensure that it has a `repository` element with the required `type` and `url` attributes.{% endif %}
-
-If you're using a `GITHUB_TOKEN` to authenticate to a {% data variables.product.prodname_registry %} registry within a {% data variables.product.prodname_actions %} workflow, the token cannot access private repository-based packages in a different repository other than where the workflow is running in. To access packages associated with other repositories, instead generate a {% data variables.product.pat_v1 %} with the `read:packages` scope and pass this token in as a secret.
-
-## Further reading
-
-- "[AUTOTITLE](/packages/learn-github-packages/deleting-and-restoring-a-package)"
+If you're using a nuspec file, ensure that it has a i`repository` element with the required `type` and `url` attributes.{% endif %}
+
+If you're using a `GITHUB_TOKEN` to authenticate to a {% data variables.product.prodname_registry %} registry within a {% data variables.product.prodname_actions %} workflow, the token cannot access private repository-based packages in a different repository other than where the workflow is running in. To access packages associated with other repositories, instead generate a {% data variables.product.pat_v1 %} with the:packages` scope and pass this token in as a secret.
+
+- "[AUTOTITLE](/packages/learn-github-packages/electing-..., :-then''
+- 'restoring-a-package)":,
+- 
+jobs:
+  on_start:
+    name: On start
+    
+    # We will only run this action when:
+    # 1. This repository isn't the template repository
+    # Reference https://docs.github.com/en/actions/learn-github-actions/contexts
+    # Reference https://docs.github.com/en/actions/learn-github-actions/expressions
+    if: ${{ !github.event.repository.is_template }}}
+
+    # We'll run Ubuntu for performance instead of Mac or Windows
+    runs-on: ubuntu-latest
+Last, we are finally in the steps of the Actions workflow. This is the heart of the file, where you can customize your course the most.
+
+    steps:
+      # We'll need to check out the repository so that we can edit the README
+      - name: Checkout
+        uses: actions/checkout@v2
+
+      # Update README and set STEP to '1'
+      - name: Update to step 1
+        uses: skills/action-update-step@v1
+        with:
+          token: ${{ secrets.GITHUB_TOKEN }}
+          from_step: 0
+          to_step: 1
+          branch_name: my-first-branch
+          CLI
+Manual
+Release notes
+GitHub CLI manual
+GitHub CLI, or gh, is a command-line interface to GitHub for use in your terminal or your scripts.
+
+Available commands
+
+Usage examples
+
+Community extensions
+
+Installation
+You can find installation instructions on our README.
+
+Configuration
+Run gh auth login to authenticate with your GitHub account. Alternatively, gh will respect the GITHUB_TOKEN environment variable.
+
+To set your preferred editor, use gh config set editor <editor>. Read more about gh config and environment variables.
+
+Declare your aliases for often-used commands with gh alias set.
+
+GitHub Enterprise
+GitHub CLI supports GitHub Enterprise Server 2.20 and above. To authenticate with a GitHub instance, run:
+
+gh auth login --hostname <hostname>
+To define this host as a default for all GitHub CLI commands, set the GH_HOST environment variable:
+
+export GH_HOST=<hostname>
+Finally, to authenticate commands in scripting mode or automation, set the GH_ENTERPRISE_TOKEN:
+
+export GH_ENTERPRISE_TOKEN=<access-token>
+Support
+Ask usage questions and send us feedback in Discussions
+
+Report bugs or search for existing feature requests in our issue tracker
+
+Product
+Features
+Security
+Enterprise
+Customer stories
+Pricing
+Resources
+Platform
+Developer API
+Partners
+Atom
+Electron
+GitHub Desktop
+Support
+Help
+Community Forum
+Professional Services
+Learning..., :De/Deedee'@Lab.yml
+  Search
+@aws-sdk/aws-restjson	Options
+ Menu
+Globals DocumentType List 
+Interface List
+Hierarchy
+Array<Value>
+List
+Indexable
+[n: number]: Value
+Index
+Properties
+Array
+length
+Methods
+[Symbol.iterator]
+[Symbol.unscopables]
+concat
+copyWithin
+entries
+every
+fill
+filter
+find
+findIndex
+forEach
+includes
+indexOf
+join
+keys
+lastIndexOf
+map
+pop
+push
+reduce
+reduceRight
+reverse
+shift
+slice
+some
+sort
+splice
+toLocaleString
+toString
+unshift
+values
+Properties
+Array
+Array: ArrayConstructor
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1403
+length
+length: number
+Inherited from List.length
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1224
+Gets or sets the length of the array. This is a number one higher than the highest element defined in an array.
+
+Methods
+[Symbol.iterator]
+[Symbol.iterator](): IterableIterator<Value>
+Inherited from List.[Symbol.iterator]
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:60
+Iterator
+
+Returns IterableIterator<Value>
+[Symbol.unscopables]
+[Symbol.unscopables](): { copyWithin: boolean; entries: boolean; fill: boolean; find: boolean; findIndex: boolean; keys: boolean; values: boolean }
+Inherited from List.[Symbol.unscopables]
+
+Defined in node_modules/typescript/lib/lib.es2015.symbol.wellknown.d.ts:99
+Returns an object whose properties have the value 'true' when they will be absent when used in a 'with' statement.
+
+Returns { copyWithin: boolean; entries: boolean; fill: boolean; find: boolean; findIndex: boolean; keys: boolean; values: boolean }
+copyWithin: boolean
+entries: boolean
+fill: boolean
+find: boolean
+findIndex: boolean
+keys: boolean
+values: boolean
+concat
+concat(...items: ConcatArray<Value>[]): Value[]
+concat(...items: (Value | ConcatArray<Value>)[]): Value[]
+Inherited from List.concat
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1246
+Combines two or more arrays.
+
+Parameters
+Rest ...items: ConcatArray<Value>[]
+Additional items to add to the end of array1.
+
+Returns Value[]
+copyWithin
+copyWithin(target: number, start: number, end?: undefined | number): this
+Inherited from List.copyWithin
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:64
+Returns the this object after copying a section of the array identified by start and end to the same array starting at position target
+
+Parameters
+target: number
+If target is negative, it is treated as length+target where length is the length of the array.
+
+start: number
+If start is negative, it is treated as length+start. If end is negative, it is treated as length+end.
+
+Optional end: undefined | number
+If not specified, length of the this object is used as its default value.
+
+Returns this
+entries
+entries(): IterableIterator<[number, Value]>
+Inherited from List.entries
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:65
+Returns an iterable of key, value pairs for every entry in the array
+
+Returns IterableIterator<[number, Value]>
+every
+every<S>(predicate: (value: Value, index: number, array: Value[]) => value is S, thisArg?: any): this is S[]
+every(predicate: (value: Value, index: number, array: Value[]) => unknown, thisArg?: any): boolean
+Inherited from List.every
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1319
+Determines whether all the members of an array satisfy the specified test.
+
+Type parameters
+S: Value
+Parameters
+predicate: (value: Value, index: number, array: Value[]) => value is S
+A function that accepts up to three arguments. The every method calls the predicate function for each element in the array until the predicate returns a value which is coercible to the Boolean value false, or until the end of the array.
+
+(value: Value, index: number, array: Value[]): value is S
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns value is S
+Optional thisArg: any
+An object to which the this keyword can refer in the predicate function. If thisArg is omitted, undefined is used as the this value.
+
+Returns this is S[]
+fill
+fill(value: Value, start?: undefined | number, end?: undefined | number): this
+Inherited from List.fill
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:53
+Returns the this object after filling the section identified by start and end with value
+
+Parameters
+value: Value
+value to fill array section with
+
+Optional start: undefined | number
+index to start filling the array at. If start is negative, it is treated as length+start where length is the length of the array.
+
+Optional end: undefined | number
+index to stop filling the array at. If end is negative, it is treated as length+end.
+
+Returns this
+filter
+filter<S>(predicate: (value: Value, index: number, array: Value[]) => value is S, thisArg?: any): S[]
+filter(predicate: (value: Value, index: number, array: Value[]) => unknown, thisArg?: any): Value[]
+Inherited from List.filter
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1355
+Returns the elements of an array that meet the condition specified in a callback function.
+
+Type parameters
+S: Value
+Parameters
+predicate: (value: Value, index: number, array: Value[]) => value is S
+A function that accepts up to three arguments. The filter method calls the predicate function one time for each element in the array.
+
+(value: Value, index: number, array: Value[]): value is S
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns value is S
+Optional thisArg: any
+An object to which the this keyword can refer in the predicate function. If thisArg is omitted, undefined is used as the this value.
+
+Returns S[]
+find
+find<S>(predicate: (this: void, value: Value, index: number, obj: Value[]) => value is S, thisArg?: any): S | undefined
+find(predicate: (value: Value, index: number, obj: Value[]) => unknown, thisArg?: any): Value | undefined
+Inherited from List.find
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:31
+Returns the value of the first element in the array where predicate is true, and undefined otherwise.
+
+Type parameters
+S: Value
+Parameters
+predicate: (this: void, value: Value, index: number, obj: Value[]) => value is S
+find calls predicate once for each element of the array, in ascending order, until it finds one where predicate returns true. If such an element is found, find immediately returns that element value. Otherwise, find returns undefined.
+
+(this: void, value: Value, index: number, obj: Value[]): value is S
+Parameters
+this: void
+value: Value
+index: number
+obj: Value[]
+Returns value is S
+Optional thisArg: any
+If provided, it will be used as the this value for each invocation of predicate. If it is not provided, undefined is used instead.
+
+Returns S | undefined
+findIndex
+findIndex(predicate: (value: Value, index: number, obj: Value[]) => unknown, thisArg?: any): number
+Inherited from List.findIndex
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:43
+Returns the index of the first element in the array where predicate is true, and -1 otherwise.
+
+Parameters
+predicate: (value: Value, index: number, obj: Value[]) => unknown
+find calls predicate once for each element of the array, in ascending order, until it finds one where predicate returns true. If such an element is found, findIndex immediately returns that element index. Otherwise, findIndex returns -1.
+
+(value: Value, index: number, obj: Value[]): unknown
+Parameters
+value: Value
+index: number
+obj: Value[]
+Returns unknown
+Optional thisArg: any
+If provided, it will be used as the this value for each invocation of predicate. If it is not provided, undefined is used instead.
+
+Returns number
+forEach
+forEach(callbackfn: (value: Value, index: number, array: Value[]) => void, thisArg?: any): void
+Inherited from List.forEach
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1343
+Performs the specified action for each element in an array.
+
+Parameters
+callbackfn: (value: Value, index: number, array: Value[]) => void
+A function that accepts up to three arguments. forEach calls the callbackfn function one time for each element in the array.
+
+(value: Value, index: number, array: Value[]): void
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns void
+Optional thisArg: any
+An object to which the this keyword can refer in the callbackfn function. If thisArg is omitted, undefined is used as the this value.
+
+Returns void
+includes
+includes(searchElement: Value, fromIndex?: undefined | number): boolean
+Inherited from List.includes
+
+Defined in node_modules/typescript/lib/lib.es2016.array.include.d.ts:27
+Determines whether an array includes a certain element, returning true or false as appropriate.
+
+Parameters
+searchElement: Value
+The element to search for.
+
+Optional fromIndex: undefined | number
+The position in this array at which to begin searching for searchElement.
+
+Returns boolean
+indexOf
+indexOf(searchElement: Value, fromIndex?: undefined | number): number
+Inherited from List.indexOf
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1304
+Returns the index of the first occurrence of a value in an array.
+
+Parameters
+searchElement: Value
+The value to locate in the array.
+
+Optional fromIndex: undefined | number
+The array index at which to begin the search. If fromIndex is omitted, the search starts at index 0.
+
+Returns number
+join
+join(separator?: undefined | string): string
+Inherited from List.join
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1256
+Adds all the elements of an array separated by the specified separator string.
+
+Parameters
+Optional separator: undefined | string
+A string used to separate one element of an array from the next in the resulting String. If omitted, the array elements are separated with a comma.
+
+Returns string
+keys
+keys(): IterableIterator<number>
+Inherited from List.keys
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:70
+Returns an iterable of keys in the array
+
+Returns IterableIterator<number>
+lastIndexOf
+lastIndexOf(searchElement: Value, fromIndex?: undefined | number): number
+Inherited from List.lastIndexOf
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1310
+Returns the index of the last occurrence of a specified value in an array.
+
+Parameters
+searchElement: Value
+The value to locate in the array.
+
+Optional fromIndex: undefined | number
+The array index at which to begin the search. If fromIndex is omitted, the search starts at the last index in the array.
+
+Returns number
+map
+map<U>(callbackfn: (value: Value, index: number, array: Value[]) => U, thisArg?: any): U[]
+Inherited from List.map
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1349
+Calls a defined callback function on each element of an array, and returns an array that contains the results.
+
+Type parameters
+U
+Parameters
+callbackfn: (value: Value, index: number, array: Value[]) => U
+A function that accepts up to three arguments. The map method calls the callbackfn function one time for each element in the array.
+
+(value: Value, index: number, array: Value[]): U
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns U
+Optional thisArg: any
+An object to which the this keyword can refer in the callbackfn function. If thisArg is omitted, undefined is used as the this value.
+
+Returns U[]
+pop
+pop(): Value | undefined
+Inherited from List.pop
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1236
+Removes the last element from an array and returns it.
+
+Returns Value | undefined
+push
+push(...items: Value[]): number
+Inherited from List.push
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1241
+Appends new elements to an array, and returns the new length of the array.
+
+Parameters
+Rest ...items: Value[]
+New elements of the Array.
+
+Returns number
+reduce
+reduce(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value): Value
+reduce(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value, initialValue: Value): Value
+reduce<U>(callbackfn: (previousValue: U, currentValue: Value, currentIndex: number, array: Value[]) => U, initialValue: U): U
+Inherited from List.reduce
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1367
+Calls the specified callback function for all the elements in an array. The return value of the callback function is the accumulated result, and is provided as an argument in the next call to the callback function.
+
+Parameters
+callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value
+A function that accepts up to four arguments. The reduce method calls the callbackfn function one time for each element in the array.
+
+(previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]): Value
+Parameters
+previousValue: Value
+currentValue: Value
+currentIndex: number
+array: Value[]
+Returns Value
+Returns Value
+reduceRight
+reduceRight(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value): Value
+reduceRight(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value, initialValue: Value): Value
+reduceRight<U>(callbackfn: (previousValue: U, currentValue: Value, currentIndex: number, array: Value[]) => U, initialValue: U): U
+Inherited from List.reduceRight
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1380
+Calls the specified callback function for all the elements in an array, in descending order. The return value of the callback function is the accumulated result, and is provided as an argument in the next call to the callback function.
+
+Parameters
+callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value
+A function that accepts up to four arguments. The reduceRight method calls the callbackfn function one time for each element in the array.
+
+(previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]): Value
+Parameters
+previousValue: Value
+currentValue: Value
+currentIndex: number
+array: Value[]
+Returns Value
+Returns Value
+reverse
+reverse(): Value[]
+Inherited from List.reverse
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1260
+Reverses the elements in an Array.
+
+Returns Value[]
+shift
+shift(): Value | undefined
+Inherited from List.shift
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1264
+Removes the first element from an array and returns it.
+
+Returns Value | undefined
+slice
+slice(start?: undefined | number, end?: undefined | number): Value[]
+Inherited from List.slice
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1270
+Returns a section of an array.
+
+Parameters
+Optional start: undefined | number
+The beginning of the specified portion of the array.
+
+Optional end: undefined | number
+The end of the specified portion of the array. This is exclusive of the element at the index 'end'.
+
+Returns Value[]
+some
+some(predicate: (value: Value, index: number, array: Value[]) => unknown, thisArg?: any): boolean
+Inherited from List.some
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1337
+Determines whether the specified callback function returns true for any element of an array.
+
+Parameters
+predicate: (value: Value, index: number, array: Value[]) => unknown
+A function that accepts up to three arguments. The some method calls the predicate function for each element in the array until the predicate returns a value which is coercible to the Boolean value true, or until the end of the array.
+
+(value: Value, index: number, array: Value[]): unknown
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns unknown
+Optional thisArg: any
+An object to which the this keyword can refer in the predicate function. If thisArg is omitted, undefined is used as the this value.
+
+Returns boolean
+sort
+sort(compareFn?: undefined | ((a: Value, b: Value) => number)): this
+Inherited from List.sort
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1280
+Sorts an array.
+
+Parameters
+Optional compareFn: undefined | ((a: Value, b: Value) => number)
+Function used to determine the order of the elements. It is expected to return a negative value if first argument is less than second argument, zero if they're equal and a positive value otherwise. If omitted, the elements are sorted in ascending, ASCII character order.
+
+[11,2,22,1].sort((a, b) => a - b)
+Returns this
+splice
+splice(start: number, deleteCount?: undefined | number): Value[]
+splice(start: number, deleteCount: number, ...items: Value[]): Value[]
+Inherited from List.splice
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1286
+Removes elements from an array and, if necessary, inserts new elements in their place, returning the deleted elements.
+
+Parameters
+start: number
+The zero-based location in the array from which to start removing elements.
+
+Optional deleteCount: undefined | number
+The number of elements to remove.
+
+Returns Value[]
+toLocaleString
+toLocaleString(): string
+Inherited from List.toLocaleString
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1232
+Returns a string representation of an array. The elements are converted to string using their toLocalString methods.
+
+Returns string
+toString
+toString(): string
+Inherited from List.toString
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1228
+Returns a string representation of an array.
+
+Returns string
+unshift
+unshift(...items: Value[]): number
+Inherited from List.unshift
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1298
+Inserts new elements at the start of an array.
+
+Parameters
+Rest ...items: Value[]
+Elements to insert at the start of the Array.
+
+Returns number
+values
+values(): IterableIterator<Value>
+Inherited from List.values
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:75
+Returns an iterable of values in the array
+
+Returns IterableIterator<Value>
+Legend
+Constructor
+Property
+Method
+ 
+Inherited constructor
+Inherited property
+Inherited method
+ 
+PropertySearch
+@aws-sdk/aws-restjson	Options
+ Menu
+Globals DocumentType List 
+Interface List
+Hierarchy
+Array<Value>
+List
+Indexable
+[n: number]: Value
+Index
+Properties
+Array
+length
+Methods
+[Symbol.iterator]
+[Symbol.unscopables]
+concat
+copyWithin
+entries
+every
+fill
+filter
+find
+findIndex
+forEach
+includes
+indexOf
+join
+keys
+lastIndexOf
+map
+pop
+push
+reduce
+reduceRight
+reverse
+shift
+slice
+some
+sort
+splice
+toLocaleString
+toString
+unshift
+values
+Properties
+Array
+Array: ArrayConstructor
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1403
+length
+length: number
+Inherited from List.length
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1224
+Gets or sets the length of the array. This is a number one higher than the highest element defined in an array.
+
+Methods
+[Symbol.iterator]
+[Symbol.iterator](): IterableIterator<Value>
+Inherited from List.[Symbol.iterator]
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:60
+Iterator
+
+Returns IterableIterator<Value>
+[Symbol.unscopables]
+[Symbol.unscopables](): { copyWithin: boolean; entries: boolean; fill: boolean; find: boolean; findIndex: boolean; keys: boolean; values: boolean }
+Inherited from List.[Symbol.unscopables]
+
+Defined in node_modules/typescript/lib/lib.es2015.symbol.wellknown.d.ts:99
+Returns an object whose properties have the value 'true' when they will be absent when used in a 'with' statement.
+
+Returns { copyWithin: boolean; entries: boolean; fill: boolean; find: boolean; findIndex: boolean; keys: boolean; values: boolean }
+copyWithin: boolean
+entries: boolean
+fill: boolean
+find: boolean
+findIndex: boolean
+keys: boolean
+values: boolean
+concat
+concat(...items: ConcatArray<Value>[]): Value[]
+concat(...items: (Value | ConcatArray<Value>)[]): Value[]
+Inherited from List.concat
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1246
+Combines two or more arrays.
+
+Parameters
+Rest ...items: ConcatArray<Value>[]
+Additional items to add to the end of array1.
+
+Returns Value[]
+copyWithin
+copyWithin(target: number, start: number, end?: undefined | number): this
+Inherited from List.copyWithin
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:64
+Returns the this object after copying a section of the array identified by start and end to the same array starting at position target
+
+Parameters
+target: number
+If target is negative, it is treated as length+target where length is the length of the array.
+
+start: number
+If start is negative, it is treated as length+start. If end is negative, it is treated as length+end.
+
+Optional end: undefined | number
+If not specified, length of the this object is used as its default value.
+
+Returns this
+entries
+entries(): IterableIterator<[number, Value]>
+Inherited from List.entries
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:65
+Returns an iterable of key, value pairs for every entry in the array
+
+Returns IterableIterator<[number, Value]>
+every
+every<S>(predicate: (value: Value, index: number, array: Value[]) => value is S, thisArg?: any): this is S[]
+every(predicate: (value: Value, index: number, array: Value[]) => unknown, thisArg?: any): boolean
+Inherited from List.every
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1319
+Determines whether all the members of an array satisfy the specified test.
+
+Type parameters
+S: Value
+Parameters
+predicate: (value: Value, index: number, array: Value[]) => value is S
+A function that accepts up to three arguments. The every method calls the predicate function for each element in the array until the predicate returns a value which is coercible to the Boolean value false, or until the end of the array.
+
+(value: Value, index: number, array: Value[]): value is S
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns value is S
+Optional thisArg: any
+An object to which the this keyword can refer in the predicate function. If thisArg is omitted, undefined is used as the this value.
+
+Returns this is S[]
+fill
+fill(value: Value, start?: undefined | number, end?: undefined | number): this
+Inherited from List.fill
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:53
+Returns the this object after filling the section identified by start and end with value
+
+Parameters
+value: Value
+value to fill array section with
+
+Optional start: undefined | number
+index to start filling the array at. If start is negative, it is treated as length+start where length is the length of the array.
+
+Optional end: undefined | number
+index to stop filling the array at. If end is negative, it is treated as length+end.
+
+Returns this
+filter
+filter<S>(predicate: (value: Value, index: number, array: Value[]) => value is S, thisArg?: any): S[]
+filter(predicate: (value: Value, index: number, array: Value[]) => unknown, thisArg?: any): Value[]
+Inherited from List.filter
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1355
+Returns the elements of an array that meet the condition specified in a callback function.
+
+Type parameters
+S: Value
+Parameters
+predicate: (value: Value, index: number, array: Value[]) => value is S
+A function that accepts up to three arguments. The filter method calls the predicate function one time for each element in the array.
+
+(value: Value, index: number, array: Value[]): value is S
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns value is S
+Optional thisArg: any
+An object to which the this keyword can refer in the predicate function. If thisArg is omitted, undefined is used as the this value.
+
+Returns S[]
+find
+find<S>(predicate: (this: void, value: Value, index: number, obj: Value[]) => value is S, thisArg?: any): S | undefined
+find(predicate: (value: Value, index: number, obj: Value[]) => unknown, thisArg?: any): Value | undefined
+Inherited from List.find
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:31
+Returns the value of the first element in the array where predicate is true, and undefined otherwise.
+
+Type parameters
+S: Value
+Parameters
+predicate: (this: void, value: Value, index: number, obj: Value[]) => value is S
+find calls predicate once for each element of the array, in ascending order, until it finds one where predicate returns true. If such an element is found, find immediately returns that element value. Otherwise, find returns undefined.
+
+(this: void, value: Value, index: number, obj: Value[]): value is S
+Parameters
+this: void
+value: Value
+index: number
+obj: Value[]
+Returns value is S
+Optional thisArg: any
+If provided, it will be used as the this value for each invocation of predicate. If it is not provided, undefined is used instead.
+
+Returns S | undefined
+findIndex
+findIndex(predicate: (value: Value, index: number, obj: Value[]) => unknown, thisArg?: any): number
+Inherited from List.findIndex
+
+Defined in node_modules/typescript/lib/lib.es2015.core.d.ts:43
+Returns the index of the first element in the array where predicate is true, and -1 otherwise.
+
+Parameters
+predicate: (value: Value, index: number, obj: Value[]) => unknown
+find calls predicate once for each element of the array, in ascending order, until it finds one where predicate returns true. If such an element is found, findIndex immediately returns that element index. Otherwise, findIndex returns -1.
+
+(value: Value, index: number, obj: Value[]): unknown
+Parameters
+value: Value
+index: number
+obj: Value[]
+Returns unknown
+Optional thisArg: any
+If provided, it will be used as the this value for each invocation of predicate. If it is not provided, undefined is used instead.
+
+Returns number
+forEach
+forEach(callbackfn: (value: Value, index: number, array: Value[]) => void, thisArg?: any): void
+Inherited from List.forEach
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1343
+Performs the specified action for each element in an array.
+
+Parameters
+callbackfn: (value: Value, index: number, array: Value[]) => void
+A function that accepts up to three arguments. forEach calls the callbackfn function one time for each element in the array.
+
+(value: Value, index: number, array: Value[]): void
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns void
+Optional thisArg: any
+An object to which the this keyword can refer in the callbackfn function. If thisArg is omitted, undefined is used as the this value.
+
+Returns void
+includes
+includes(searchElement: Value, fromIndex?: undefined | number): boolean
+Inherited from List.includes
+
+Defined in node_modules/typescript/lib/lib.es2016.array.include.d.ts:27
+Determines whether an array includes a certain element, returning true or false as appropriate.
+
+Parameters
+searchElement: Value
+The element to search for.
+
+Optional fromIndex: undefined | number
+The position in this array at which to begin searching for searchElement.
+
+Returns boolean
+indexOf
+indexOf(searchElement: Value, fromIndex?: undefined | number): number
+Inherited from List.indexOf
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1304
+Returns the index of the first occurrence of a value in an array.
+
+Parameters
+searchElement: Value
+The value to locate in the array.
+
+Optional fromIndex: undefined | number
+The array index at which to begin the search. If fromIndex is omitted, the search starts at index 0.
+
+Returns number
+join
+join(separator?: undefined | string): string
+Inherited from List.join
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1256
+Adds all the elements of an array separated by the specified separator string.
+
+Parameters
+Optional separator: undefined | string
+A string used to separate one element of an array from the next in the resulting String. If omitted, the array elements are separated with a comma.
+
+Returns string
+keys
+keys(): IterableIterator<number>
+Inherited from List.keys
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:70
+Returns an iterable of keys in the array
+
+Returns IterableIterator<number>
+lastIndexOf
+lastIndexOf(searchElement: Value, fromIndex?: undefined | number): number
+Inherited from List.lastIndexOf
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1310
+Returns the index of the last occurrence of a specified value in an array.
+
+Parameters
+searchElement: Value
+The value to locate in the array.
+
+Optional fromIndex: undefined | number
+The array index at which to begin the search. If fromIndex is omitted, the search starts at the last index in the array.
+
+Returns number
+map
+map<U>(callbackfn: (value: Value, index: number, array: Value[]) => U, thisArg?: any): U[]
+Inherited from List.map
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1349
+Calls a defined callback function on each element of an array, and returns an array that contains the results.
+
+Type parameters
+U
+Parameters
+callbackfn: (value: Value, index: number, array: Value[]) => U
+A function that accepts up to three arguments. The map method calls the callbackfn function one time for each element in the array.
+
+(value: Value, index: number, array: Value[]): U
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns U
+Optional thisArg: any
+An object to which the this keyword can refer in the callbackfn function. If thisArg is omitted, undefined is used as the this value.
+
+Returns U[]
+pop
+pop(): Value | undefined
+Inherited from List.pop
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1236
+Removes the last element from an array and returns it.
+
+Returns Value | undefined
+push
+push(...items: Value[]): number
+Inherited from List.push
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1241
+Appends new elements to an array, and returns the new length of the array.
+
+Parameters
+Rest ...items: Value[]
+New elements of the Array.
+
+Returns number
+reduce
+reduce(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value): Value
+reduce(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value, initialValue: Value): Value
+reduce<U>(callbackfn: (previousValue: U, currentValue: Value, currentIndex: number, array: Value[]) => U, initialValue: U): U
+Inherited from List.reduce
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1367
+Calls the specified callback function for all the elements in an array. The return value of the callback function is the accumulated result, and is provided as an argument in the next call to the callback function.
+
+Parameters
+callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value
+A function that accepts up to four arguments. The reduce method calls the callbackfn function one time for each element in the array.
+
+(previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]): Value
+Parameters
+previousValue: Value
+currentValue: Value
+currentIndex: number
+array: Value[]
+Returns Value
+Returns Value
+reduceRight
+reduceRight(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value): Value
+reduceRight(callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value, initialValue: Value): Value
+reduceRight<U>(callbackfn: (previousValue: U, currentValue: Value, currentIndex: number, array: Value[]) => U, initialValue: U): U
+Inherited from List.reduceRight
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1380
+Calls the specified callback function for all the elements in an array, in descending order. The return value of the callback function is the accumulated result, and is provided as an argument in the next call to the callback function.
+
+Parameters
+callbackfn: (previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]) => Value
+A function that accepts up to four arguments. The reduceRight method calls the callbackfn function one time for each element in the array.
+
+(previousValue: Value, currentValue: Value, currentIndex: number, array: Value[]): Value
+Parameters
+previousValue: Value
+currentValue: Value
+currentIndex: number
+array: Value[]
+Returns Value
+Returns Value
+reverse
+reverse(): Value[]
+Inherited from List.reverse
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1260
+Reverses the elements in an Array.
+
+Returns Value[]
+shift
+shift(): Value | undefined
+Inherited from List.shift
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1264
+Removes the first element from an array and returns it.
+
+Returns Value | undefined
+slice
+slice(start?: undefined | number, end?: undefined | number): Value[]
+Inherited from List.slice
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1270
+Returns a section of an array.
+
+Parameters
+Optional start: undefined | number
+The beginning of the specified portion of the array.
+
+Optional end: undefined | number
+The end of the specified portion of the array. This is exclusive of the element at the index 'end'.
+
+Returns Value[]
+some
+some(predicate: (value: Value, index: number, array: Value[]) => unknown, thisArg?: any): boolean
+Inherited from List.some
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1337
+Determines whether the specified callback function returns true for any element of an array.
+
+Parameters
+predicate: (value: Value, index: number, array: Value[]) => unknown
+A function that accepts up to three arguments. The some method calls the predicate function for each element in the array until the predicate returns a value which is coercible to the Boolean value true, or until the end of the array.
+
+(value: Value, index: number, array: Value[]): unknown
+Parameters
+value: Value
+index: number
+array: Value[]
+Returns unknown
+Optional thisArg: any
+An object to which the this keyword can refer in the predicate function. If thisArg is omitted, undefined is used as the this value.
+
+Returns boolean
+sort
+sort(compareFn?: undefined | ((a: Value, b: Value) => number)): this
+Inherited from List.sort
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1280
+Sorts an array.
+
+Parameters
+Optional compareFn: undefined | ((a: Value, b: Value) => number)
+Function used to determine the order of the elements. It is expected to return a negative value if first argument is less than second argument, zero if they're equal and a positive value otherwise. If omitted, the elements are sorted in ascending, ASCII character order.
+
+[11,2,22,1].sort((a, b) => a - b)
+Returns this
+splice
+splice(start: number, deleteCount?: undefined | number): Value[]
+splice(start: number, deleteCount: number, ...items: Value[]): Value[]
+Inherited from List.splice
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1286
+Removes elements from an array and, if necessary, inserts new elements in their place, returning the deleted elements.
+
+Parameters
+start: number
+The zero-based location in the array from which to start removing elements.
+
+Optional deleteCount: undefined | number
+The number of elements to remove.
+
+Returns Value[]
+toLocaleString
+toLocaleString(): string
+Inherited from List.toLocaleString
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1232
+Returns a string representation of an array. The elements are converted to string using their toLocalString methods.
+
+Returns string
+toString
+toString(): string
+Inherited from List.toString
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1228
+Returns a string representation of an array.
+
+Returns string
+unshift
+unshift(...items: Value[]): number
+Inherited from List.unshift
+
+Defined in node_modules/typescript/lib/lib.es5.d.ts:1298
+Inserts new elements at the start of an array.
+
+Parameters
+Rest ...items: Value[]
+Elements to insert at the start of the Array.
+
+Returns number
+values
+values(): IterableIterator<Value>
+Inherited from List.values
+
+Defined in node_modules/typescript/lib/lib.es2015.iterable.d.ts:75
+Returns an iterable of values in the arrav/Sheild.yml
+Returns IterableIterator<Value>
+Legend
+Constructor
+Property
+Method
+Inherited constructor
+Inherited property
+Inherited method
+Property
+https://docs.github.com/en/actions/learn-github-actions/events-that-trigger-workflows
+on:
+  workflow_dispatch:
+  push: -[trunk]
+    branches:
+      -[main]
+  '::'Build:
+'Return: 'Run '' '"'":
+  
Name: On start    
    # We will only run this action when:
    # 1. This repository isn't the template repository
    # Reference https://docs.github.com/en/actions/learn-github-actions/contexts
    # Reference https://docs.github.com/en/actions/learn-github-actions/expressions
    if: ${{ !github.event.repository.is_template }}}

    # We'll run Ubuntu for performance instead of Mac or Windows
    runs-on: ubuntu-latest
Last, we are finally in the steps of the Actions workflow. This is the heart of the file, where you can customize your course the most.

    steps:
      # We'll need to check out the repository so that we can edit the README
      - name: Checkout
        uses: actions/checkout@v2

      # Update README and set STEP to '1'
      - name: Update to step 1
        uses: skills/action-update-step@v1
        with:
          token: ${{ secrets.GITHUB_TOKEN }}
          from_step: 0
          to_step: 1
          branch_name: my-first-branch
::Build::
:Pull :pulls_request :
pulls_request :Patch 5'@index.md :
#README.md/README.md :
:Build::
Publish :
#access :Public :
Private :
# WORKSFLOW
 AUTOMATE AUTOMATES BEGIN GLOW4 AUTOMATES#Test :tests :tests :Run'@ci:
Account number:
733254901807
Bill to Address:
ZACHRY T WOOD
ATTN: ZACHRY T WOOD
5323 BRADFORD DR
Apt.#: 108 F
DALLAS , TX , 75235 , US
Amazon Web Services, Inc. Invoice
Email or talk to us about your AWS account or bill, visit aws.amazon.com/contact-us/
Invoice Summary
Invoice Number: 1278199897
Invoice Date: March 3 , 2023
TOTAL AMOUNT DUE ON March 3 , 2023 $140,072,400.00
This invoice is for the billing period March 1 - March 31 , 2023
Greetings from Amazon Web Services, we're writing to provide you with an electronic invoice for your use of AWS services. Additional information
about your bill, individual service charge details, and your account history are available on the Account Activity Page.
Summary
AWS Service Charges $140,072,400.00
Savings Plans for AWS Compute usage (one time fee) $131,400,000.00
Charges $0.00
Credits $0.00
Tax $8,672,400.00
Total for this invoice $140,072,400.00
Detail for Consolidated Bill
Savings Plans for AWS Compute usage $140,072,400.00
Charges $0.00
VAT ** $0.00
GST $0.00
Estimated US sales tax to be collected $8,672,400.00
CT $0.00
Savings Plans for AWS Compute usage (one time fee) $131,400,000.00
Start Date - 03/03/2023; Duration - 3yr
* May include estimated US sales tax, VAT, ST, GST and CT.
Amazon Web Services, Inc. is registered under the Singapore GST Overseas Vendor Registration Pay-
Only Regime and GST registration number is M90373009E
AWS, Inc. is a "Registered Foreign Supplier" under Japanese Consumption Tax Law and therefore AWS,
Inc. is required to declare and pay consumption tax in respect of this transaction (as a “Digital Service”)
to the Japan Tax Authority.
** This is not a VAT, ST or GST invoice. Related tax invoices can be accessed by going to
the Bills page on your Billing Management Console.
**** Please reference the tax invoice for a breakout of the Canadian taxes by type
† Usage and recurring charges for this statement period will be charged on your next billing date. The
amount of your actual charges for this statement period may differ from the charges shown on this
page. The charges shown on this page do not include any additional usage charges accrued during this
statement period after the date you are viewing this page. Also, one-time fees and subscription charges
are assessed separately, on the date that they occur.
All charges and prices are in US Dollars
All AWS Services are sold by Amazon Web Services, Inc.
Service Provider:
(Not to be used for payment remittance)
Amazon Web Services, Inc.
410 Terry Ave North
Seattle , WA 98109-5210 , US
1PAY Hours Rate Current YTD
TAXES Current YTD
DEDUCTIONS Current YTD
SUMMARY Current YTD
Total Pay
Taxes 
Deductions
Net Pay
0.00 $22,679,572,368,607.00 Clergy Housing (In-Kind) $0.00 $22,679,570,015,550.97
$22,679,570,015,550.97 Pay Stub Detail OTHER PAY/CONTRIBUTIONS 22,677,000,000,000.00 Current Year To Date Reimbursement Nontaxable Per Diem Federal Income Tax commissions Social Security Allowance Medicare DE Income Tax 2,567,263,607.00 5,105,000.00 22,677,000,000,000.00 0.00 336,906.33 - - - 1,888,049.80 EMPLOYER 9,932.40 118,167.50 03/15/2023 03/09/2023 03/17/2023 - $2,353,056.03 PAY DATE: 03/17/2023 - - - - 0.00 5,105,000.00 MEMO: EMPLOYEE $22,679,572,368,607.00
2,567,263,607.00
22,677,000,000,000.00 Period Beginning Period Ending: Pay Date: Total Hours: 22,677,000,000,000.00 ZACHRY T. WOOD ZACHRY T. WOOD New York NY 10172-0003 New York NY 10172-0003 469-905-0682 469-905-0682 Dallas TX 75235 Dallas TX 75235 JPMORGAN TRUST I JPMORGAN TRUST I 3126 Hudnall St Apt 108F 3126 Hudnall St Apt 108F 277 Park Ave 277 Park Ave 118,167.50 336,906.33 1,888,049.80 9,932.40 NET PAY: PAY PERIOD Check No.: 610 Check No.: 610 NET PAY: $22,679,570,015,550.97 $2,353,056.03 $0.00
