# api documentation for  [knockout (v3.4.2)](http://knockoutjs.com/)  [![npm package](https://img.shields.io/npm/v/npmdoc-knockout.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-knockout) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-knockout.svg)](https://travis-ci.org/npmdoc/node-npmdoc-knockout)
#### Knockout makes it easier to create rich, responsive UIs with JavaScript

[![NPM](https://nodei.co/npm/knockout.png?downloads=true)](https://www.npmjs.com/package/knockout)

[![apidoc](https://npmdoc.github.io/node-npmdoc-knockout/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-knockout_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-knockout/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-knockout/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-knockout/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "The Knockout.js team"
    },
    "bugs": {
        "url": "https://github.com/knockout/knockout/issues"
    },
    "dependencies": {},
    "description": "Knockout makes it easier to create rich, responsive UIs with JavaScript",
    "devDependencies": {
        "closure-compiler": "~0.2.1",
        "grunt": "~0.4.1",
        "grunt-cli": "~0.1.0"
    },
    "directories": {},
    "dist": {
        "shasum": "e87958de77ad1e936f7ce645bab8b5d7c456d937",
        "tarball": "https://registry.npmjs.org/knockout/-/knockout-3.4.2.tgz"
    },
    "gitHead": "4888305843439159bf100bd74e41768fd8650d1d",
    "homepage": "http://knockoutjs.com/",
    "license": "MIT",
    "licenses": [
        {
            "type": "MIT",
            "url": "http://www.opensource.org/licenses/mit-license.php"
        }
    ],
    "main": "build/output/knockout-latest.debug.js",
    "maintainers": [
        {
            "name": "mtscout6",
            "email": "mtscout6@gmail.com"
        },
        {
            "name": "stevesanderson",
            "email": "steve@codeville.net"
        },
        {
            "name": "mbest",
            "email": "mbest@dasya.com"
        }
    ],
    "name": "knockout",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/knockout/knockout.git"
    },
    "scripts": {
        "prepublish": "grunt",
        "test": "node spec/runner.node.js"
    },
    "testling": {
        "preprocess": "build/build.sh",
        "html": "spec/runner.html?src=build/output/knockout-latest.js&testling=true",
        "browsers": [
            "ie/6..latest",
            "chrome/20..latest",
            "firefox/3..latest",
            "safari/5.0.5..latest",
            "opera/11.0..latest",
            "iphone/6..latest",
            "ipad/6..latest"
        ]
    },
    "version": "3.4.2"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module knockout](#apidoc.module.knockout)
1.  [function <span class="apidocSignatureSpan">knockout.</span>__tr_ambtns (bindings, nodeName)](#apidoc.element.knockout.__tr_ambtns)
1.  [function <span class="apidocSignatureSpan">knockout.</span>applyBindingAccessorsToNode (node, bindings, viewModelOrBindingContext)](#apidoc.element.knockout.applyBindingAccessorsToNode)
1.  [function <span class="apidocSignatureSpan">knockout.</span>applyBindings (viewModelOrBindingContext, rootNode)](#apidoc.element.knockout.applyBindings)
1.  [function <span class="apidocSignatureSpan">knockout.</span>applyBindingsToDescendants (viewModelOrBindingContext, rootNode)](#apidoc.element.knockout.applyBindingsToDescendants)
1.  [function <span class="apidocSignatureSpan">knockout.</span>applyBindingsToNode (node, bindings, viewModelOrBindingContext)](#apidoc.element.knockout.applyBindingsToNode)
1.  [function <span class="apidocSignatureSpan">knockout.</span>bindingContext (dataItemOrAccessor, parentContext, dataItemAlias, extendCallback, options)](#apidoc.element.knockout.bindingContext)
1.  [function <span class="apidocSignatureSpan">knockout.</span>bindingProvider ()](#apidoc.element.knockout.bindingProvider)
1.  [function <span class="apidocSignatureSpan">knockout.</span>cleanNode (node)](#apidoc.element.knockout.cleanNode)
1.  [function <span class="apidocSignatureSpan">knockout.</span>computed (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.computed)
1.  [function <span class="apidocSignatureSpan">knockout.</span>contextFor (node)](#apidoc.element.knockout.contextFor)
1.  [function <span class="apidocSignatureSpan">knockout.</span>dataFor (node)](#apidoc.element.knockout.dataFor)
1.  [function <span class="apidocSignatureSpan">knockout.</span>dependentObservable (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.dependentObservable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>exportProperty (owner, publicName, object)](#apidoc.element.knockout.exportProperty)
1.  [function <span class="apidocSignatureSpan">knockout.</span>exportSymbol (koPath, object)](#apidoc.element.knockout.exportSymbol)
1.  [function <span class="apidocSignatureSpan">knockout.</span>getBindingHandler (bindingKey)](#apidoc.element.knockout.getBindingHandler)
1.  [function <span class="apidocSignatureSpan">knockout.</span>hasPrototype (instance, prototype)](#apidoc.element.knockout.hasPrototype)
1.  [function <span class="apidocSignatureSpan">knockout.</span>ignoreDependencies (callback, callbackTarget, callbackArgs)](#apidoc.element.knockout.ignoreDependencies)
1.  [function <span class="apidocSignatureSpan">knockout.</span>isComputed (instance)](#apidoc.element.knockout.isComputed)
1.  [function <span class="apidocSignatureSpan">knockout.</span>isObservable (instance)](#apidoc.element.knockout.isObservable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>isPureComputed (instance)](#apidoc.element.knockout.isPureComputed)
1.  [function <span class="apidocSignatureSpan">knockout.</span>isSubscribable (instance)](#apidoc.element.knockout.isSubscribable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>isWritableObservable (instance)](#apidoc.element.knockout.isWritableObservable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>isWriteableObservable (instance)](#apidoc.element.knockout.isWriteableObservable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>jqueryTmplTemplateEngine ()](#apidoc.element.knockout.jqueryTmplTemplateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>nativeTemplateEngine ()](#apidoc.element.knockout.nativeTemplateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>observable (initialValue)](#apidoc.element.knockout.observable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>observableArray (initialValues)](#apidoc.element.knockout.observableArray)
1.  [function <span class="apidocSignatureSpan">knockout.</span>pureComputed (evaluatorFunctionOrOptions, evaluatorFunctionTarget)](#apidoc.element.knockout.pureComputed)
1.  [function <span class="apidocSignatureSpan">knockout.</span>removeNode (node)](#apidoc.element.knockout.removeNode)
1.  [function <span class="apidocSignatureSpan">knockout.</span>renderTemplate (template, dataOrBindingContext, options, targetNodeOrNodeArray, renderMode)](#apidoc.element.knockout.renderTemplate)
1.  [function <span class="apidocSignatureSpan">knockout.</span>renderTemplateForEach (template, arrayOrObservableArray, options, targetNode, parentBindingContext)](#apidoc.element.knockout.renderTemplateForEach)
1.  [function <span class="apidocSignatureSpan">knockout.</span>setTemplateEngine (templateEngine)](#apidoc.element.knockout.setTemplateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>storedBindingContextForNode (node, bindingContext)](#apidoc.element.knockout.storedBindingContextForNode)
1.  [function <span class="apidocSignatureSpan">knockout.</span>subscribable ()](#apidoc.element.knockout.subscribable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>subscription (target, callback, disposeCallback)](#apidoc.element.knockout.subscription)
1.  [function <span class="apidocSignatureSpan">knockout.</span>templateEngine ()](#apidoc.element.knockout.templateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>templateSources.anonymousTemplate (element)](#apidoc.element.knockout.templateSources.anonymousTemplate)
1.  [function <span class="apidocSignatureSpan">knockout.</span>templateSources.domElement (element)](#apidoc.element.knockout.templateSources.domElement)
1.  [function <span class="apidocSignatureSpan">knockout.</span>toJS (rootObject)](#apidoc.element.knockout.toJS)
1.  [function <span class="apidocSignatureSpan">knockout.</span>toJSON (rootObject, replacer, space)](#apidoc.element.knockout.toJSON)
1.  [function <span class="apidocSignatureSpan">knockout.</span>unwrap (value)](#apidoc.element.knockout.unwrap)
1.  object <span class="apidocSignatureSpan">knockout.</span>bindingContext.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>bindingHandlers
1.  object <span class="apidocSignatureSpan">knockout.</span>bindingProvider.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>components
1.  object <span class="apidocSignatureSpan">knockout.</span>components.defaultLoader
1.  object <span class="apidocSignatureSpan">knockout.</span>computedContext
1.  object <span class="apidocSignatureSpan">knockout.</span>dependencyDetection
1.  object <span class="apidocSignatureSpan">knockout.</span>dependentObservable.fn
1.  object <span class="apidocSignatureSpan">knockout.</span>expressionRewriting
1.  object <span class="apidocSignatureSpan">knockout.</span>expressionRewriting.bindingRewriteValidators
1.  object <span class="apidocSignatureSpan">knockout.</span>extenders
1.  object <span class="apidocSignatureSpan">knockout.</span>jqueryTmplTemplateEngine.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>jsonExpressionRewriting
1.  object <span class="apidocSignatureSpan">knockout.</span>memoization
1.  object <span class="apidocSignatureSpan">knockout.</span>nativeTemplateEngine.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>options
1.  object <span class="apidocSignatureSpan">knockout.</span>selectExtensions
1.  object <span class="apidocSignatureSpan">knockout.</span>subscription.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>tasks
1.  object <span class="apidocSignatureSpan">knockout.</span>templateEngine.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>templateRewriting
1.  object <span class="apidocSignatureSpan">knockout.</span>templateSources
1.  object <span class="apidocSignatureSpan">knockout.</span>templateSources.anonymousTemplate.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>templateSources.domElement.prototype
1.  object <span class="apidocSignatureSpan">knockout.</span>utils
1.  object <span class="apidocSignatureSpan">knockout.</span>utils.domData
1.  object <span class="apidocSignatureSpan">knockout.</span>utils.domNodeDisposal
1.  object <span class="apidocSignatureSpan">knockout.</span>virtualElements
1.  string <span class="apidocSignatureSpan">knockout.</span>version

#### [module knockout.bindingContext](#apidoc.module.knockout.bindingContext)
1.  [function <span class="apidocSignatureSpan">knockout.</span>bindingContext (dataItemOrAccessor, parentContext, dataItemAlias, extendCallback, options)](#apidoc.element.knockout.bindingContext.bindingContext)

#### [module knockout.bindingContext.prototype](#apidoc.module.knockout.bindingContext.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.bindingContext.prototype.</span>createChildContext (dataItemOrAccessor, dataItemAlias, extendCallback, options)](#apidoc.element.knockout.bindingContext.prototype.createChildContext)
1.  [function <span class="apidocSignatureSpan">knockout.bindingContext.prototype.</span>createStaticChildContext (dataItemOrAccessor, dataItemAlias)](#apidoc.element.knockout.bindingContext.prototype.createStaticChildContext)
1.  [function <span class="apidocSignatureSpan">knockout.bindingContext.prototype.</span>extend (properties)](#apidoc.element.knockout.bindingContext.prototype.extend)

#### [module knockout.bindingProvider](#apidoc.module.knockout.bindingProvider)
1.  [function <span class="apidocSignatureSpan">knockout.</span>bindingProvider ()](#apidoc.element.knockout.bindingProvider.bindingProvider)
1.  object <span class="apidocSignatureSpan">knockout.bindingProvider.</span>instance

#### [module knockout.bindingProvider.prototype](#apidoc.module.knockout.bindingProvider.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>getBindingAccessors (node, bindingContext)](#apidoc.element.knockout.bindingProvider.prototype.getBindingAccessors)
1.  [function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>getBindings (node, bindingContext)](#apidoc.element.knockout.bindingProvider.prototype.getBindings)
1.  [function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>getBindingsString (node, bindingContext)](#apidoc.element.knockout.bindingProvider.prototype.getBindingsString)
1.  [function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>nodeHasBindings (node)](#apidoc.element.knockout.bindingProvider.prototype.nodeHasBindings)
1.  [function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>parseBindingsString (bindingsString, bindingContext, node, options)](#apidoc.element.knockout.bindingProvider.prototype.parseBindingsString)

#### [module knockout.components](#apidoc.module.knockout.components)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>_getFirstResultFromLoaders (methodName, argsExceptCallback, callback, candidateLoaders)](#apidoc.element.knockout.components._getFirstResultFromLoaders)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>addBindingsForCustomElement (allBindings, node, bindingContext, valueAccessors)](#apidoc.element.knockout.components.addBindingsForCustomElement)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>clearCachedDefinition (componentName)](#apidoc.element.knockout.components.clearCachedDefinition)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>get (componentName, callback)](#apidoc.element.knockout.components.get)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>getComponentNameForNode (node)](#apidoc.element.knockout.components.getComponentNameForNode)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>isRegistered (componentName)](#apidoc.element.knockout.components.isRegistered)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>register (componentName, config)](#apidoc.element.knockout.components.register)
1.  [function <span class="apidocSignatureSpan">knockout.components.</span>unregister (componentName)](#apidoc.element.knockout.components.unregister)
1.  object <span class="apidocSignatureSpan">knockout.components.</span>_allRegisteredComponents
1.  object <span class="apidocSignatureSpan">knockout.components.</span>defaultLoader
1.  object <span class="apidocSignatureSpan">knockout.components.</span>loaders

#### [module knockout.components.defaultLoader](#apidoc.module.knockout.components.defaultLoader)
1.  [function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>getConfig (componentName, callback)](#apidoc.element.knockout.components.defaultLoader.getConfig)
1.  [function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>loadComponent (componentName, config, callback)](#apidoc.element.knockout.components.defaultLoader.loadComponent)
1.  [function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>loadTemplate (componentName, templateConfig, callback)](#apidoc.element.knockout.components.defaultLoader.loadTemplate)
1.  [function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>loadViewModel (componentName, viewModelConfig, callback)](#apidoc.element.knockout.components.defaultLoader.loadViewModel)

#### [module knockout.dependencyDetection](#apidoc.module.knockout.dependencyDetection)
1.  [function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>begin (options)](#apidoc.element.knockout.dependencyDetection.begin)
1.  [function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>end ()](#apidoc.element.knockout.dependencyDetection.end)
1.  [function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>getDependenciesCount ()](#apidoc.element.knockout.dependencyDetection.getDependenciesCount)
1.  [function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>ignore (callback, callbackTarget, callbackArgs)](#apidoc.element.knockout.dependencyDetection.ignore)
1.  [function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>isInitial ()](#apidoc.element.knockout.dependencyDetection.isInitial)
1.  [function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>registerDependency (subscribable)](#apidoc.element.knockout.dependencyDetection.registerDependency)

#### [module knockout.dependentObservable](#apidoc.module.knockout.dependentObservable)
1.  [function <span class="apidocSignatureSpan">knockout.</span>dependentObservable (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.dependentObservable.dependentObservable)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.</span>__ko_proto__ (initialValue)](#apidoc.element.knockout.dependentObservable.__ko_proto__)
1.  object <span class="apidocSignatureSpan">knockout.dependentObservable.</span>fn

#### [module knockout.dependentObservable.fn](#apidoc.module.knockout.dependentObservable.fn)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>__ko_proto__ (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.dependentObservable.fn.__ko_proto__)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>addDependencyTracking (id, target, trackingObj)](#apidoc.element.knockout.dependentObservable.fn.addDependencyTracking)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>dispose ()](#apidoc.element.knockout.dependentObservable.fn.dispose)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>equalityComparer (a, b)](#apidoc.element.knockout.dependentObservable.fn.equalityComparer)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluateImmediate (notifyChange)](#apidoc.element.knockout.dependentObservable.fn.evaluateImmediate)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluateImmediate_CallReadThenEndDependencyDetection (state, dependencyDetectionContext)](#apidoc.element.knockout.dependentObservable.fn.evaluateImmediate_CallReadThenEndDependencyDetection)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluateImmediate_CallReadWithDependencyDetection (notifyChange)](#apidoc.element.knockout.dependentObservable.fn.evaluateImmediate_CallReadWithDependencyDetection)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluatePossiblyAsync ()](#apidoc.element.knockout.dependentObservable.fn.evaluatePossiblyAsync)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>getDependenciesCount ()](#apidoc.element.knockout.dependentObservable.fn.getDependenciesCount)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>haveDependenciesChanged ()](#apidoc.element.knockout.dependentObservable.fn.haveDependenciesChanged)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>isActive ()](#apidoc.element.knockout.dependentObservable.fn.isActive)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>limit (limitFunction)](#apidoc.element.knockout.dependentObservable.fn.limit)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>markDirty ()](#apidoc.element.knockout.dependentObservable.fn.markDirty)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>peek (evaluate)](#apidoc.element.knockout.dependentObservable.fn.peek)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>respondToChange ()](#apidoc.element.knockout.dependentObservable.fn.respondToChange)
1.  [function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>subscribeToDependency (target)](#apidoc.element.knockout.dependentObservable.fn.subscribeToDependency)

#### [module knockout.expressionRewriting](#apidoc.module.knockout.expressionRewriting)
1.  [function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>insertPropertyAccessorsIntoJson (bindingsStringOrKeyValueArray, bindingOptions)](#apidoc.element.knockout.expressionRewriting.insertPropertyAccessorsIntoJson)
1.  [function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>keyValueArrayContainsKey (keyValueArray, key)](#apidoc.element.knockout.expressionRewriting.keyValueArrayContainsKey)
1.  [function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>parseObjectLiteral (objectLiteralString)](#apidoc.element.knockout.expressionRewriting.parseObjectLiteral)
1.  [function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>preProcessBindings (bindingsStringOrKeyValueArray, bindingOptions)](#apidoc.element.knockout.expressionRewriting.preProcessBindings)
1.  [function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>writeValueToProperty (property, allBindings, key, value, checkIfDifferent)](#apidoc.element.knockout.expressionRewriting.writeValueToProperty)
1.  object <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>_twoWayBindings
1.  object <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>bindingRewriteValidators
1.  object <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>twoWayBindings

#### [module knockout.expressionRewriting.bindingRewriteValidators](#apidoc.module.knockout.expressionRewriting.bindingRewriteValidators)
1.  boolean <span class="apidocSignatureSpan">knockout.expressionRewriting.bindingRewriteValidators.</span>foreach
1.  boolean <span class="apidocSignatureSpan">knockout.expressionRewriting.bindingRewriteValidators.</span>if
1.  boolean <span class="apidocSignatureSpan">knockout.expressionRewriting.bindingRewriteValidators.</span>ifnot
1.  boolean <span class="apidocSignatureSpan">knockout.expressionRewriting.bindingRewriteValidators.</span>with
1.  [function <span class="apidocSignatureSpan">knockout.expressionRewriting.bindingRewriteValidators.</span>template (bindingValue)](#apidoc.element.knockout.expressionRewriting.bindingRewriteValidators.template)

#### [module knockout.extenders](#apidoc.module.knockout.extenders)
1.  [function <span class="apidocSignatureSpan">knockout.extenders.</span>deferred (target, options)](#apidoc.element.knockout.extenders.deferred)
1.  [function <span class="apidocSignatureSpan">knockout.extenders.</span>notify (target, notifyWhen)](#apidoc.element.knockout.extenders.notify)
1.  [function <span class="apidocSignatureSpan">knockout.extenders.</span>rateLimit (target, options)](#apidoc.element.knockout.extenders.rateLimit)
1.  [function <span class="apidocSignatureSpan">knockout.extenders.</span>throttle (target, timeout)](#apidoc.element.knockout.extenders.throttle)
1.  [function <span class="apidocSignatureSpan">knockout.extenders.</span>trackArrayChanges (target, options)](#apidoc.element.knockout.extenders.trackArrayChanges)

#### [module knockout.jqueryTmplTemplateEngine](#apidoc.module.knockout.jqueryTmplTemplateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>jqueryTmplTemplateEngine ()](#apidoc.element.knockout.jqueryTmplTemplateEngine.jqueryTmplTemplateEngine)

#### [module knockout.jqueryTmplTemplateEngine.prototype](#apidoc.module.knockout.jqueryTmplTemplateEngine.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.jqueryTmplTemplateEngine.prototype.</span>constructor ()](#apidoc.element.knockout.jqueryTmplTemplateEngine.prototype.constructor)

#### [module knockout.memoization](#apidoc.module.knockout.memoization)
1.  [function <span class="apidocSignatureSpan">knockout.memoization.</span>memoize (callback)](#apidoc.element.knockout.memoization.memoize)
1.  [function <span class="apidocSignatureSpan">knockout.memoization.</span>parseMemoText (memoText)](#apidoc.element.knockout.memoization.parseMemoText)
1.  [function <span class="apidocSignatureSpan">knockout.memoization.</span>unmemoize (memoId, callbackParams)](#apidoc.element.knockout.memoization.unmemoize)
1.  [function <span class="apidocSignatureSpan">knockout.memoization.</span>unmemoizeDomNodeAndDescendants (domNode, extraCallbackParamsArray)](#apidoc.element.knockout.memoization.unmemoizeDomNodeAndDescendants)

#### [module knockout.nativeTemplateEngine](#apidoc.module.knockout.nativeTemplateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>nativeTemplateEngine ()](#apidoc.element.knockout.nativeTemplateEngine.nativeTemplateEngine)
1.  object <span class="apidocSignatureSpan">knockout.nativeTemplateEngine.</span>instance

#### [module knockout.nativeTemplateEngine.prototype](#apidoc.module.knockout.nativeTemplateEngine.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.nativeTemplateEngine.prototype.</span>constructor ()](#apidoc.element.knockout.nativeTemplateEngine.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">knockout.nativeTemplateEngine.prototype.</span>renderTemplateSource (templateSource, bindingContext, options, templateDocument)](#apidoc.element.knockout.nativeTemplateEngine.prototype.renderTemplateSource)

#### [module knockout.selectExtensions](#apidoc.module.knockout.selectExtensions)
1.  [function <span class="apidocSignatureSpan">knockout.selectExtensions.</span>readValue (element)](#apidoc.element.knockout.selectExtensions.readValue)
1.  [function <span class="apidocSignatureSpan">knockout.selectExtensions.</span>writeValue (element, value, allowUnset)](#apidoc.element.knockout.selectExtensions.writeValue)

#### [module knockout.subscription](#apidoc.module.knockout.subscription)
1.  [function <span class="apidocSignatureSpan">knockout.</span>subscription (target, callback, disposeCallback)](#apidoc.element.knockout.subscription.subscription)

#### [module knockout.subscription.prototype](#apidoc.module.knockout.subscription.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.subscription.prototype.</span>dispose ()](#apidoc.element.knockout.subscription.prototype.dispose)

#### [module knockout.tasks](#apidoc.module.knockout.tasks)
1.  [function <span class="apidocSignatureSpan">knockout.tasks.</span>cancel (handle)](#apidoc.element.knockout.tasks.cancel)
1.  [function <span class="apidocSignatureSpan">knockout.tasks.</span>resetForTesting ()](#apidoc.element.knockout.tasks.resetForTesting)
1.  [function <span class="apidocSignatureSpan">knockout.tasks.</span>runEarly ()](#apidoc.element.knockout.tasks.runEarly)
1.  [function <span class="apidocSignatureSpan">knockout.tasks.</span>schedule (func)](#apidoc.element.knockout.tasks.schedule)
1.  [function <span class="apidocSignatureSpan">knockout.tasks.</span>scheduler (callback)](#apidoc.element.knockout.tasks.scheduler)

#### [module knockout.templateEngine](#apidoc.module.knockout.templateEngine)
1.  [function <span class="apidocSignatureSpan">knockout.</span>templateEngine ()](#apidoc.element.knockout.templateEngine.templateEngine)

#### [module knockout.templateEngine.prototype](#apidoc.module.knockout.templateEngine.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>createJavaScriptEvaluatorBlock (script)](#apidoc.element.knockout.templateEngine.prototype.createJavaScriptEvaluatorBlock)
1.  [function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>isTemplateRewritten (template, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.isTemplateRewritten)
1.  [function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>makeTemplateSource (template, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.makeTemplateSource)
1.  [function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>renderTemplate (template, bindingContext, options, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.renderTemplate)
1.  [function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>renderTemplateSource (templateSource, bindingContext, options, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.renderTemplateSource)
1.  [function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>rewriteTemplate (template, rewriterCallback, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.rewriteTemplate)

#### [module knockout.templateRewriting](#apidoc.module.knockout.templateRewriting)
1.  [function <span class="apidocSignatureSpan">knockout.templateRewriting.</span>applyMemoizedBindingsToNextSibling (bindings, nodeName)](#apidoc.element.knockout.templateRewriting.applyMemoizedBindingsToNextSibling)
1.  [function <span class="apidocSignatureSpan">knockout.templateRewriting.</span>ensureTemplateIsRewritten (template, templateEngine, templateDocument)](#apidoc.element.knockout.templateRewriting.ensureTemplateIsRewritten)
1.  [function <span class="apidocSignatureSpan">knockout.templateRewriting.</span>memoizeBindingAttributeSyntax (htmlString, templateEngine)](#apidoc.element.knockout.templateRewriting.memoizeBindingAttributeSyntax)

#### [module knockout.templateSources](#apidoc.module.knockout.templateSources)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.</span>anonymousTemplate (element)](#apidoc.element.knockout.templateSources.anonymousTemplate)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.</span>domElement (element)](#apidoc.element.knockout.templateSources.domElement)

#### [module knockout.templateSources.anonymousTemplate](#apidoc.module.knockout.templateSources.anonymousTemplate)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.</span>anonymousTemplate (element)](#apidoc.element.knockout.templateSources.anonymousTemplate.anonymousTemplate)

#### [module knockout.templateSources.anonymousTemplate.prototype](#apidoc.module.knockout.templateSources.anonymousTemplate.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.anonymousTemplate.prototype.</span>constructor (element)](#apidoc.element.knockout.templateSources.anonymousTemplate.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.anonymousTemplate.prototype.</span>text ()](#apidoc.element.knockout.templateSources.anonymousTemplate.prototype.text)

#### [module knockout.templateSources.domElement](#apidoc.module.knockout.templateSources.domElement)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.</span>domElement (element)](#apidoc.element.knockout.templateSources.domElement.domElement)

#### [module knockout.templateSources.domElement.prototype](#apidoc.module.knockout.templateSources.domElement.prototype)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.domElement.prototype.</span>data (key)](#apidoc.element.knockout.templateSources.domElement.prototype.data)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.domElement.prototype.</span>nodes ()](#apidoc.element.knockout.templateSources.domElement.prototype.nodes)
1.  [function <span class="apidocSignatureSpan">knockout.templateSources.domElement.prototype.</span>text ()](#apidoc.element.knockout.templateSources.domElement.prototype.text)

#### [module knockout.utils](#apidoc.module.knockout.utils)
1.  boolean <span class="apidocSignatureSpan">knockout.utils.</span>canSetPrototype
1.  boolean <span class="apidocSignatureSpan">knockout.utils.</span>isIe6
1.  boolean <span class="apidocSignatureSpan">knockout.utils.</span>isIe7
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>addOrRemoveItem (array, value, included)](#apidoc.element.knockout.utils.addOrRemoveItem)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>anyDomNodeIsAttachedToDocument (nodes)](#apidoc.element.knockout.utils.anyDomNodeIsAttachedToDocument)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayFilter (array, predicate)](#apidoc.element.knockout.utils.arrayFilter)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayFirst (array, predicate, predicateOwner)](#apidoc.element.knockout.utils.arrayFirst)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayForEach (array, action)](#apidoc.element.knockout.utils.arrayForEach)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayGetDistinctValues (array)](#apidoc.element.knockout.utils.arrayGetDistinctValues)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayIndexOf (array, item)](#apidoc.element.knockout.utils.arrayIndexOf)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayMap (array, mapping)](#apidoc.element.knockout.utils.arrayMap)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayPushAll (array, valuesToPush)](#apidoc.element.knockout.utils.arrayPushAll)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>arrayRemoveItem (array, itemToRemove)](#apidoc.element.knockout.utils.arrayRemoveItem)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>catchFunctionErrors (delegate)](#apidoc.element.knockout.utils.catchFunctionErrors)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>cloneNodes (nodesArray, shouldCleanNodes)](#apidoc.element.knockout.utils.cloneNodes)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>compareArrays (oldArray, newArray, options)](#apidoc.element.knockout.utils.compareArrays)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>createSymbolOrString (identifier)](#apidoc.element.knockout.utils.createSymbolOrString)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>deferError (error)](#apidoc.element.knockout.utils.deferError)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>domNodeIsAttachedToDocument (node)](#apidoc.element.knockout.utils.domNodeIsAttachedToDocument)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>domNodeIsContainedBy (node, containedByNode)](#apidoc.element.knockout.utils.domNodeIsContainedBy)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>emptyDomNode (domNode)](#apidoc.element.knockout.utils.emptyDomNode)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>ensureSelectElementIsRenderedCorrectly (selectElement)](#apidoc.element.knockout.utils.ensureSelectElementIsRenderedCorrectly)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>extend (target, source)](#apidoc.element.knockout.utils.extend)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>findMovesInArrayComparison (left, right, limitFailedCompares)](#apidoc.element.knockout.utils.findMovesInArrayComparison)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>fixUpContinuousNodeArray (continuousNodeArray, parentNode)](#apidoc.element.knockout.utils.fixUpContinuousNodeArray)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>forceRefresh (node)](#apidoc.element.knockout.utils.forceRefresh)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>getFormFields (form, fieldName)](#apidoc.element.knockout.utils.getFormFields)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>makeArray (arrayLikeObject)](#apidoc.element.knockout.utils.makeArray)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>moveCleanedNodesToContainerElement (nodes)](#apidoc.element.knockout.utils.moveCleanedNodesToContainerElement)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>objectForEach (obj, action)](#apidoc.element.knockout.utils.objectForEach)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>objectMap (source, mapping)](#apidoc.element.knockout.utils.objectMap)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>parseHtmlFragment (html, documentContext)](#apidoc.element.knockout.utils.parseHtmlFragment)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>parseJson (jsonString)](#apidoc.element.knockout.utils.parseJson)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>peekObservable (value)](#apidoc.element.knockout.utils.peekObservable)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>postJson (urlOrForm, data, options)](#apidoc.element.knockout.utils.postJson)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>range (min, max)](#apidoc.element.knockout.utils.range)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>registerEventHandler (element, eventType, handler)](#apidoc.element.knockout.utils.registerEventHandler)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>replaceDomNodes (nodeToReplaceOrNodeArray, newNodesArray)](#apidoc.element.knockout.utils.replaceDomNodes)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setDomNodeChildren (domNode, childNodes)](#apidoc.element.knockout.utils.setDomNodeChildren)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setDomNodeChildrenFromArrayMapping (domNode, array, mapping, options, callbackAfterAddingNodes)](#apidoc.element.knockout.utils.setDomNodeChildrenFromArrayMapping)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setElementName (element, name)](#apidoc.element.knockout.utils.setElementName)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setHtml (node, html)](#apidoc.element.knockout.utils.setHtml)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setOptionNodeSelectionState (optionNode, isSelected)](#apidoc.element.knockout.utils.setOptionNodeSelectionState)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setPrototypeOf (obj, proto)](#apidoc.element.knockout.utils.setPrototypeOf)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setPrototypeOfOrExtend (obj, proto)](#apidoc.element.knockout.utils.setPrototypeOfOrExtend)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setTextContent (element, textContent)](#apidoc.element.knockout.utils.setTextContent)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>setTimeout (handler, timeout)](#apidoc.element.knockout.utils.setTimeout)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>stringStartsWith (string, startsWith)](#apidoc.element.knockout.utils.stringStartsWith)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>stringTrim (string)](#apidoc.element.knockout.utils.stringTrim)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>stringifyJson (data, replacer, space)](#apidoc.element.knockout.utils.stringifyJson)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>tagNameLower (element)](#apidoc.element.knockout.utils.tagNameLower)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>toggleDomNodeCssClass (node, classNames, shouldHaveClass)](#apidoc.element.knockout.utils.toggleDomNodeCssClass)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>triggerEvent (element, eventType)](#apidoc.element.knockout.utils.triggerEvent)
1.  [function <span class="apidocSignatureSpan">knockout.utils.</span>unwrapObservable (value)](#apidoc.element.knockout.utils.unwrapObservable)
1.  object <span class="apidocSignatureSpan">knockout.utils.</span>domData
1.  object <span class="apidocSignatureSpan">knockout.utils.</span>domNodeDisposal
1.  object <span class="apidocSignatureSpan">knockout.utils.</span>fieldsIncludedWithJsonPost

#### [module knockout.utils.domData](#apidoc.module.knockout.utils.domData)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domData.</span>clear (node)](#apidoc.element.knockout.utils.domData.clear)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domData.</span>get (node, key)](#apidoc.element.knockout.utils.domData.get)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domData.</span>nextKey ()](#apidoc.element.knockout.utils.domData.nextKey)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domData.</span>set (node, key, value)](#apidoc.element.knockout.utils.domData.set)

#### [module knockout.utils.domNodeDisposal](#apidoc.module.knockout.utils.domNodeDisposal)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>addDisposeCallback (node, callback)](#apidoc.element.knockout.utils.domNodeDisposal.addDisposeCallback)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>cleanExternalData (node)](#apidoc.element.knockout.utils.domNodeDisposal.cleanExternalData)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>cleanNode (node)](#apidoc.element.knockout.utils.domNodeDisposal.cleanNode)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>removeDisposeCallback (node, callback)](#apidoc.element.knockout.utils.domNodeDisposal.removeDisposeCallback)
1.  [function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>removeNode (node)](#apidoc.element.knockout.utils.domNodeDisposal.removeNode)

#### [module knockout.virtualElements](#apidoc.module.knockout.virtualElements)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>childNodes (node)](#apidoc.element.knockout.virtualElements.childNodes)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>emptyNode (node)](#apidoc.element.knockout.virtualElements.emptyNode)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>firstChild (node)](#apidoc.element.knockout.virtualElements.firstChild)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>hasBindingValue (node)](#apidoc.element.knockout.virtualElements.hasBindingValue)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>insertAfter (containerNode, nodeToInsert, insertAfterNode)](#apidoc.element.knockout.virtualElements.insertAfter)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>nextSibling (node)](#apidoc.element.knockout.virtualElements.nextSibling)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>normaliseVirtualElementDomStructure (elementVerified)](#apidoc.element.knockout.virtualElements.normaliseVirtualElementDomStructure)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>prepend (containerNode, nodeToPrepend)](#apidoc.element.knockout.virtualElements.prepend)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>setDomNodeChildren (node, childNodes)](#apidoc.element.knockout.virtualElements.setDomNodeChildren)
1.  [function <span class="apidocSignatureSpan">knockout.virtualElements.</span>virtualNodeBindingValue (node)](#apidoc.element.knockout.virtualElements.virtualNodeBindingValue)
1.  object <span class="apidocSignatureSpan">knockout.virtualElements.</span>allowedBindings



# <a name="apidoc.module.knockout"></a>[module knockout](#apidoc.module.knockout)

#### <a name="apidoc.element.knockout.__tr_ambtns"></a>[function <span class="apidocSignatureSpan">knockout.</span>__tr_ambtns (bindings, nodeName)](#apidoc.element.knockout.__tr_ambtns)
- description and source-code
```javascript
__tr_ambtns = function (bindings, nodeName) {
    return ko.memoization.memoize(function (domNode, bindingContext) {
        var nodeToBind = domNode.nextSibling;
        if (nodeToBind && nodeToBind.nodeName.toLowerCase() === nodeName) {
            ko.applyBindingAccessorsToNode(nodeToBind, bindings, bindingContext);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.applyBindingAccessorsToNode"></a>[function <span class="apidocSignatureSpan">knockout.</span>applyBindingAccessorsToNode (node, bindings, viewModelOrBindingContext)](#apidoc.element.knockout.applyBindingAccessorsToNode)
- description and source-code
```javascript
applyBindingAccessorsToNode = function (node, bindings, viewModelOrBindingContext) {
    if (node.nodeType === 1) // If it's an element, workaround IE <= 8 HTML parsing weirdness
        ko.virtualElements.normaliseVirtualElementDomStructure(node);
    return applyBindingsToNodeInternal(node, bindings, getBindingContext(viewModelOrBindingContext), true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.applyBindings"></a>[function <span class="apidocSignatureSpan">knockout.</span>applyBindings (viewModelOrBindingContext, rootNode)](#apidoc.element.knockout.applyBindings)
- description and source-code
```javascript
applyBindings = function (viewModelOrBindingContext, rootNode) {
    // If jQuery is loaded after Knockout, we won't initially have access to it. So save it here.
    if (!jQueryInstance && window['jQuery']) {
        jQueryInstance = window['jQuery'];
    }

    if (rootNode && (rootNode.nodeType !== 1) && (rootNode.nodeType !== 8))
        throw new Error("ko.applyBindings: first parameter should be your view model; second parameter should be a DOM node");
    rootNode = rootNode || window.document.body; // Make "rootNode" parameter optional

    applyBindingsToNodeAndDescendantsInternal(getBindingContext(viewModelOrBindingContext), rootNode, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.applyBindingsToDescendants"></a>[function <span class="apidocSignatureSpan">knockout.</span>applyBindingsToDescendants (viewModelOrBindingContext, rootNode)](#apidoc.element.knockout.applyBindingsToDescendants)
- description and source-code
```javascript
applyBindingsToDescendants = function (viewModelOrBindingContext, rootNode) {
    if (rootNode.nodeType === 1 || rootNode.nodeType === 8)
        applyBindingsToDescendantsInternal(getBindingContext(viewModelOrBindingContext), rootNode, true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.applyBindingsToNode"></a>[function <span class="apidocSignatureSpan">knockout.</span>applyBindingsToNode (node, bindings, viewModelOrBindingContext)](#apidoc.element.knockout.applyBindingsToNode)
- description and source-code
```javascript
applyBindingsToNode = function (node, bindings, viewModelOrBindingContext) {
    var context = getBindingContext(viewModelOrBindingContext);
    return ko.applyBindingAccessorsToNode(node, makeBindingAccessors(bindings, context, node), context);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingContext"></a>[function <span class="apidocSignatureSpan">knockout.</span>bindingContext (dataItemOrAccessor, parentContext, dataItemAlias, extendCallback, options)](#apidoc.element.knockout.bindingContext)
- description and source-code
```javascript
bindingContext = function (dataItemOrAccessor, parentContext, dataItemAlias, extendCallback, options) {

    // The binding context object includes static properties for the current, parent, and root view models.
    // If a view model is actually stored in an observable, the corresponding binding context object, and
    // any child contexts, must be updated when the view model is changed.
    function updateContext() {
        // Most of the time, the context will directly get a view model object, but if a function is given,
        // we call the function to retrieve the view model. If the function accesses any observables or returns
        // an observable, the dependency is tracked, and those observables can later cause the binding
        // context to be updated.
        var dataItemOrObservable = isFunc ? dataItemOrAccessor() : dataItemOrAccessor,
            dataItem = ko.utils.unwrapObservable(dataItemOrObservable);

        if (parentContext) {
            // When a "parent" context is given, register a dependency on the parent context. Thus whenever the
            // parent context is updated, this context will also be updated.
            if (parentContext._subscribable)
                parentContext._subscribable();

            // Copy $root and any custom properties from the parent context
            ko.utils.extend(self, parentContext);

            // Because the above copy overwrites our own properties, we need to reset them.
            self._subscribable = subscribable;
        } else {
            self['$parents'] = [];
            self['$root'] = dataItem;

            // Export 'ko' in the binding context so it will be available in bindings and templates
            // even if 'ko' isn't exported as a global, such as when using an AMD loader.
            // See https://github.com/SteveSanderson/knockout/issues/490
            self['ko'] = ko;
        }
        self['$rawData'] = dataItemOrObservable;
        self['$data'] = dataItem;
        if (dataItemAlias)
            self[dataItemAlias] = dataItem;

        // The extendCallback function is provided when creating a child context or extending a context.
        // It handles the specific actions needed to finish setting up the binding context. Actions in this
        // function could also add dependencies to this binding context.
        if (extendCallback)
            extendCallback(self, parentContext, dataItem);

        return self['$data'];
    }
    function disposeWhen() {
        return nodes && !ko.utils.anyDomNodeIsAttachedToDocument(nodes);
    }

    var self = this,
        isFunc = typeof(dataItemOrAccessor) == "function" && !ko.isObservable(dataItemOrAccessor),
        nodes,
        subscribable;

    if (options && options['exportDependencies']) {
        // The "exportDependencies" option means that the calling code will track any dependencies and re-create
        // the binding context when they change.
        updateContext();
    } else {
        subscribable = ko.dependentObservable(updateContext, null, { disposeWhen: disposeWhen, disposeWhenNodeIsRemoved: true });

        // At this point, the binding context has been initialized, and the "subscribable" computed observable is
        // subscribed to any observables that were accessed in the process. If there is nothing to track, the
        // computed will be inactive, and we can safely throw it away. If it's active, the computed is stored in
        // the context object.
        if (subscribable.isActive()) {
            self._subscribable = subscribable;

            // Always notify because even if the model ($data) hasn't changed, other context properties might have changed
            subscribable['equalityComparer'] = null;

            // We need to be able to dispose of this computed observable when it's no longer needed. This would be
            // easy if we had a single node to watch, but binding contexts can be used by many different nodes, and
            // we cannot assume that those nodes have any relation to each other. So instead we track any node that ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingProvider"></a>[function <span class="apidocSignatureSpan">knockout.</span>bindingProvider ()](#apidoc.element.knockout.bindingProvider)
- description and source-code
```javascript
bindingProvider = function () {
    this.bindingCache = {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.cleanNode"></a>[function <span class="apidocSignatureSpan">knockout.</span>cleanNode (node)](#apidoc.element.knockout.cleanNode)
- description and source-code
```javascript
cleanNode = function (node) {
    // First clean this node, where applicable
    if (cleanableNodeTypes[node.nodeType]) {
        cleanSingleNode(node);

        // ... then its descendants, where applicable
        if (cleanableNodeTypesWithDescendants[node.nodeType]) {
            // Clone the descendants list in case it changes during iteration
            var descendants = [];
            ko.utils.arrayPushAll(descendants, node.getElementsByTagName("*"));
            for (var i = 0, j = descendants.length; i < j; i++)
                cleanSingleNode(descendants[i]);
        }
    }
    return node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.computed"></a>[function <span class="apidocSignatureSpan">knockout.</span>computed (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.computed)
- description and source-code
```javascript
computed = function (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options) {
    if (typeof evaluatorFunctionOrOptions === "object") {
        // Single-parameter syntax - everything is on this "options" param
        options = evaluatorFunctionOrOptions;
    } else {
        // Multi-parameter syntax - construct the options according to the params passed
        options = options || {};
        if (evaluatorFunctionOrOptions) {
            options["read"] = evaluatorFunctionOrOptions;
        }
    }
    if (typeof options["read"] != "function")
        throw Error("Pass a function that returns the value of the ko.computed");

    var writeFunction = options["write"];
    var state = {
        latestValue: undefined,
        isStale: true,
        isDirty: true,
        isBeingEvaluated: false,
        suppressDisposalUntilDisposeWhenReturnsFalse: false,
        isDisposed: false,
        pure: false,
        isSleeping: false,
        readFunction: options["read"],
        evaluatorFunctionTarget: evaluatorFunctionTarget || options["owner"],
        disposeWhenNodeIsRemoved: options["disposeWhenNodeIsRemoved"] || options.disposeWhenNodeIsRemoved || null,
        disposeWhen: options["disposeWhen"] || options.disposeWhen,
        domNodeDisposalCallback: null,
        dependencyTracking: {},
        dependenciesCount: 0,
        evaluationTimeoutInstance: null
    };

    function computedObservable() {
        if (arguments.length > 0) {
            if (typeof writeFunction === "function") {
                // Writing a value
                writeFunction.apply(state.evaluatorFunctionTarget, arguments);
            } else {
                throw new Error("Cannot write a value to a ko.computed unless you specify a 'write' option. If you wish to read
the current value, don't pass any parameters.");
            }
            return this; // Permits chained assignments
        } else {
            // Reading the value
            ko.dependencyDetection.registerDependency(computedObservable);
            if (state.isDirty || (state.isSleeping && computedObservable.haveDependenciesChanged())) {
                computedObservable.evaluateImmediate();
            }
            return state.latestValue;
        }
    }

    computedObservable[computedState] = state;
    computedObservable.hasWriteFunction = typeof writeFunction === "function";

    // Inherit from 'subscribable'
    if (!ko.utils.canSetPrototype) {
        // 'subscribable' won't be on the prototype chain unless we put it there directly
        ko.utils.extend(computedObservable, ko.subscribable['fn']);
    }
    ko.subscribable['fn'].init(computedObservable);

    // Inherit from 'computed'
    ko.utils.setPrototypeOfOrExtend(computedObservable, computedFn);

    if (options['pure']) {
        state.pure = true;
        state.isSleeping = true;     // Starts off sleeping; will awake on the first subscription
        ko.utils.extend(computedObservable, pureComputedOverrides);
    } else if (options['deferEvaluation']) {
        ko.utils.extend(computedObservable, deferEvaluationOverrides);
    }

    if (ko.options['deferUpdates']) {
        ko.extenders['deferred'](computedObservable, true);
    }

    if (DEBUG) {
        // #1731 - Aid debugging by exposing the computed's options
        computedObservable["_options"] = options;
    }

    if (state.disposeWhenNodeIsRemoved) {
        // Since this computed is associated with a DOM node, and we don't want to dispose the computed
        // until the DOM node is *removed* from the document (as opposed to never having been in the document),
        // we'll prevent disposal until "disposeWhen" first returns false.
        state.suppressDisposalUntilDisposeWhenReturnsFalse = true;

        // disposeWhenNodeIsRemoved: true can be used to opt into the "only dispose after first false result"
        // behaviour even if there's no specific node to watch. In that case, clear the option so we don't try
        // to watch for a non-node's disposal. This technique is intended for KO's internal use only and shouldn't ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.contextFor"></a>[function <span class="apidocSignatureSpan">knockout.</span>contextFor (node)](#apidoc.element.knockout.contextFor)
- description and source-code
```javascript
contextFor = function (node) {
    // We can only do something meaningful for elements and comment nodes (in particular, not text nodes, as IE can't store domdata
 for them)
    switch (node.nodeType) {
        case 1:
        case 8:
            var context = ko.storedBindingContextForNode(node);
            if (context) return context;
            if (node.parentNode) return ko.contextFor(node.parentNode);
            break;
    }
    return undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dataFor"></a>[function <span class="apidocSignatureSpan">knockout.</span>dataFor (node)](#apidoc.element.knockout.dataFor)
- description and source-code
```javascript
dataFor = function (node) {
    var context = ko.contextFor(node);
    return context ? context['$data'] : undefined;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable"></a>[function <span class="apidocSignatureSpan">knockout.</span>dependentObservable (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.dependentObservable)
- description and source-code
```javascript
dependentObservable = function (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options) {
    if (typeof evaluatorFunctionOrOptions === "object") {
        // Single-parameter syntax - everything is on this "options" param
        options = evaluatorFunctionOrOptions;
    } else {
        // Multi-parameter syntax - construct the options according to the params passed
        options = options || {};
        if (evaluatorFunctionOrOptions) {
            options["read"] = evaluatorFunctionOrOptions;
        }
    }
    if (typeof options["read"] != "function")
        throw Error("Pass a function that returns the value of the ko.computed");

    var writeFunction = options["write"];
    var state = {
        latestValue: undefined,
        isStale: true,
        isDirty: true,
        isBeingEvaluated: false,
        suppressDisposalUntilDisposeWhenReturnsFalse: false,
        isDisposed: false,
        pure: false,
        isSleeping: false,
        readFunction: options["read"],
        evaluatorFunctionTarget: evaluatorFunctionTarget || options["owner"],
        disposeWhenNodeIsRemoved: options["disposeWhenNodeIsRemoved"] || options.disposeWhenNodeIsRemoved || null,
        disposeWhen: options["disposeWhen"] || options.disposeWhen,
        domNodeDisposalCallback: null,
        dependencyTracking: {},
        dependenciesCount: 0,
        evaluationTimeoutInstance: null
    };

    function computedObservable() {
        if (arguments.length > 0) {
            if (typeof writeFunction === "function") {
                // Writing a value
                writeFunction.apply(state.evaluatorFunctionTarget, arguments);
            } else {
                throw new Error("Cannot write a value to a ko.computed unless you specify a 'write' option. If you wish to read
the current value, don't pass any parameters.");
            }
            return this; // Permits chained assignments
        } else {
            // Reading the value
            ko.dependencyDetection.registerDependency(computedObservable);
            if (state.isDirty || (state.isSleeping && computedObservable.haveDependenciesChanged())) {
                computedObservable.evaluateImmediate();
            }
            return state.latestValue;
        }
    }

    computedObservable[computedState] = state;
    computedObservable.hasWriteFunction = typeof writeFunction === "function";

    // Inherit from 'subscribable'
    if (!ko.utils.canSetPrototype) {
        // 'subscribable' won't be on the prototype chain unless we put it there directly
        ko.utils.extend(computedObservable, ko.subscribable['fn']);
    }
    ko.subscribable['fn'].init(computedObservable);

    // Inherit from 'computed'
    ko.utils.setPrototypeOfOrExtend(computedObservable, computedFn);

    if (options['pure']) {
        state.pure = true;
        state.isSleeping = true;     // Starts off sleeping; will awake on the first subscription
        ko.utils.extend(computedObservable, pureComputedOverrides);
    } else if (options['deferEvaluation']) {
        ko.utils.extend(computedObservable, deferEvaluationOverrides);
    }

    if (ko.options['deferUpdates']) {
        ko.extenders['deferred'](computedObservable, true);
    }

    if (DEBUG) {
        // #1731 - Aid debugging by exposing the computed's options
        computedObservable["_options"] = options;
    }

    if (state.disposeWhenNodeIsRemoved) {
        // Since this computed is associated with a DOM node, and we don't want to dispose the computed
        // until the DOM node is *removed* from the document (as opposed to never having been in the document),
        // we'll prevent disposal until "disposeWhen" first returns false.
        state.suppressDisposalUntilDisposeWhenReturnsFalse = true;

        // disposeWhenNodeIsRemoved: true can be used to opt into the "only dispose after first false result"
        // behaviour even if there's no specific node to watch. In that case, clear the option so we don't try
        // to watch for a non-node's disposal. This technique is intended for KO's internal use only and shouldn't ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.exportProperty"></a>[function <span class="apidocSignatureSpan">knockout.</span>exportProperty (owner, publicName, object)](#apidoc.element.knockout.exportProperty)
- description and source-code
```javascript
exportProperty = function (owner, publicName, object) {
    owner[publicName] = object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.exportSymbol"></a>[function <span class="apidocSignatureSpan">knockout.</span>exportSymbol (koPath, object)](#apidoc.element.knockout.exportSymbol)
- description and source-code
```javascript
exportSymbol = function (koPath, object) {
    var tokens = koPath.split(".");

    // In the future, "ko" may become distinct from "koExports" (so that non-exported objects are not reachable)
    // At that point, "target" would be set to: (typeof koExports !== "undefined" ? koExports : ko)
    var target = ko;

    for (var i = 0; i < tokens.length - 1; i++)
        target = target[tokens[i]];
    target[tokens[tokens.length - 1]] = object;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.getBindingHandler"></a>[function <span class="apidocSignatureSpan">knockout.</span>getBindingHandler (bindingKey)](#apidoc.element.knockout.getBindingHandler)
- description and source-code
```javascript
getBindingHandler = function (bindingKey) {
    return ko.bindingHandlers[bindingKey];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.hasPrototype"></a>[function <span class="apidocSignatureSpan">knockout.</span>hasPrototype (instance, prototype)](#apidoc.element.knockout.hasPrototype)
- description and source-code
```javascript
hasPrototype = function (instance, prototype) {
    if ((instance === null) || (instance === undefined) || (instance[protoProperty] === undefined)) return false;
    if (instance[protoProperty] === prototype) return true;
    return ko.hasPrototype(instance[protoProperty], prototype); // Walk the prototype chain
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.ignoreDependencies"></a>[function <span class="apidocSignatureSpan">knockout.</span>ignoreDependencies (callback, callbackTarget, callbackArgs)](#apidoc.element.knockout.ignoreDependencies)
- description and source-code
```javascript
ignoreDependencies = function (callback, callbackTarget, callbackArgs) {
    try {
        begin();
        return callback.apply(callbackTarget, callbackArgs || []);
    } finally {
        end();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.isComputed"></a>[function <span class="apidocSignatureSpan">knockout.</span>isComputed (instance)](#apidoc.element.knockout.isComputed)
- description and source-code
```javascript
isComputed = function (instance) {
    return ko.hasPrototype(instance, ko.computed);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.isObservable"></a>[function <span class="apidocSignatureSpan">knockout.</span>isObservable (instance)](#apidoc.element.knockout.isObservable)
- description and source-code
```javascript
isObservable = function (instance) {
    return ko.hasPrototype(instance, ko.observable);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.isPureComputed"></a>[function <span class="apidocSignatureSpan">knockout.</span>isPureComputed (instance)](#apidoc.element.knockout.isPureComputed)
- description and source-code
```javascript
isPureComputed = function (instance) {
    return ko.hasPrototype(instance, ko.computed)
        && instance[computedState] && instance[computedState].pure;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.isSubscribable"></a>[function <span class="apidocSignatureSpan">knockout.</span>isSubscribable (instance)](#apidoc.element.knockout.isSubscribable)
- description and source-code
```javascript
isSubscribable = function (instance) {
    return instance != null && typeof instance.subscribe == "function" && typeof instance["notifySubscribers"] == "function";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.isWritableObservable"></a>[function <span class="apidocSignatureSpan">knockout.</span>isWritableObservable (instance)](#apidoc.element.knockout.isWritableObservable)
- description and source-code
```javascript
isWritableObservable = function (instance) {
    // Observable
    if ((typeof instance == 'function') && instance[protoProperty] === ko.observable)
        return true;
    // Writeable dependent observable
    if ((typeof instance == 'function') && (instance[protoProperty] === ko.dependentObservable) && (instance.hasWriteFunction))
        return true;
    // Anything else
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.isWriteableObservable"></a>[function <span class="apidocSignatureSpan">knockout.</span>isWriteableObservable (instance)](#apidoc.element.knockout.isWriteableObservable)
- description and source-code
```javascript
isWriteableObservable = function (instance) {
    // Observable
    if ((typeof instance == 'function') && instance[protoProperty] === ko.observable)
        return true;
    // Writeable dependent observable
    if ((typeof instance == 'function') && (instance[protoProperty] === ko.dependentObservable) && (instance.hasWriteFunction))
        return true;
    // Anything else
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.jqueryTmplTemplateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>jqueryTmplTemplateEngine ()](#apidoc.element.knockout.jqueryTmplTemplateEngine)
- description and source-code
```javascript
jqueryTmplTemplateEngine = function () {
    // Detect which version of jquery-tmpl you're using. Unfortunately jquery-tmpl
    // doesn't expose a version number, so we have to infer it.
    // Note that as of Knockout 1.3, we only support jQuery.tmpl 1.0.0pre and later,
    // which KO internally refers to as version "2", so older versions are no longer detected.
    var jQueryTmplVersion = this.jQueryTmplVersion = (function() {
        if (!jQueryInstance || !(jQueryInstance['tmpl']))
            return 0;
        // Since it exposes no official version number, we use our own numbering system. To be updated as jquery-tmpl evolves.
        try {
            if (jQueryInstance['tmpl']['tag']['tmpl']['open'].toString().indexOf('__') >= 0) {
                // Since 1.0.0pre, custom tags should append markup to an array called "__"
                return 2; // Final version of jquery.tmpl
            }
        } catch(ex) { /* Apparently not the version we were looking for */ }

        return 1; // Any older version that we don't support
    })();

    function ensureHasReferencedJQueryTemplates() {
        if (jQueryTmplVersion < 2)
            throw new Error("Your version of jQuery.tmpl is too old. Please upgrade to jQuery.tmpl 1.0.0pre or later.");
    }

    function executeTemplate(compiledTemplate, data, jQueryTemplateOptions) {
        return jQueryInstance['tmpl'](compiledTemplate, data, jQueryTemplateOptions);
    }

    this['renderTemplateSource'] = function(templateSource, bindingContext, options, templateDocument) {
        templateDocument = templateDocument || document;
        options = options || {};
        ensureHasReferencedJQueryTemplates();

        // Ensure we have stored a precompiled version of this template (don't want to reparse on every render)
        var precompiled = templateSource['data']('precompiled');
        if (!precompiled) {
            var templateText = templateSource['text']() || "";
            // Wrap in "with($whatever.koBindingContext) { ... }"
            templateText = "{{ko_with $item.koBindingContext}}" + templateText + "{{/ko_with}}";

            precompiled = jQueryInstance['template'](null, templateText);
            templateSource['data']('precompiled', precompiled);
        }

        var data = [bindingContext['$data']]; // Prewrap the data in an array to stop jquery.tmpl from trying to unwrap any arrays
        var jQueryTemplateOptions = jQueryInstance['extend']({ 'koBindingContext': bindingContext }, options['templateOptions']);

        var resultNodes = executeTemplate(precompiled, data, jQueryTemplateOptions);
        resultNodes['appendTo'](templateDocument.createElement("div")); // Using "appendTo" forces jQuery/jQuery.tmpl to perform
 necessary cleanup work

        jQueryInstance['fragments'] = {}; // Clear jQuery's fragment cache to avoid a memory leak after a large number of template
 renders
        return resultNodes;
    };

    this['createJavaScriptEvaluatorBlock'] = function(script) {
        return "{{ko_code ((function() { return " + script + " })()) }}";
    };

    this['addTemplate'] = function(templateName, templateMarkup) {
        document.write("<script type='text/html' id='" + templateName + "'>" + templateMarkup + "<" + "/script>");
    };

    if (jQueryTmplVersion > 0) {
        jQueryInstance['tmpl']['tag']['ko_code'] = {
            open: "__.push($1 || '');"
        };
        jQueryInstance['tmpl']['tag']['ko_with'] = {
            open: "with($1) {",
            close: "} "
        };
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.nativeTemplateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>nativeTemplateEngine ()](#apidoc.element.knockout.nativeTemplateEngine)
- description and source-code
```javascript
nativeTemplateEngine = function () {
    this['allowTemplateRewriting'] = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.observable"></a>[function <span class="apidocSignatureSpan">knockout.</span>observable (initialValue)](#apidoc.element.knockout.observable)
- description and source-code
```javascript
observable = function (initialValue) {
    function observable() {
        if (arguments.length > 0) {
            // Write

            // Ignore writes if the value hasn't changed
            if (observable.isDifferent(observable[observableLatestValue], arguments[0])) {
                observable.valueWillMutate();
                observable[observableLatestValue] = arguments[0];
                observable.valueHasMutated();
            }
            return this; // Permits chained assignments
        }
        else {
            // Read
            ko.dependencyDetection.registerDependency(observable); // The caller only needs to be notified of changes if they did
 a "read" operation
            return observable[observableLatestValue];
        }
    }

    observable[observableLatestValue] = initialValue;

    // Inherit from 'subscribable'
    if (!ko.utils.canSetPrototype) {
        // 'subscribable' won't be on the prototype chain unless we put it there directly
        ko.utils.extend(observable, ko.subscribable['fn']);
    }
    ko.subscribable['fn'].init(observable);

    // Inherit from 'observable'
    ko.utils.setPrototypeOfOrExtend(observable, observableFn);

    if (ko.options['deferUpdates']) {
        ko.extenders['deferred'](observable, true);
    }

    return observable;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.observableArray"></a>[function <span class="apidocSignatureSpan">knockout.</span>observableArray (initialValues)](#apidoc.element.knockout.observableArray)
- description and source-code
```javascript
observableArray = function (initialValues) {
    initialValues = initialValues || [];

    if (typeof initialValues != 'object' || !('length' in initialValues))
        throw new Error("The argument passed when initializing an observable array must be an array, or null, or undefined.");

    var result = ko.observable(initialValues);
    ko.utils.setPrototypeOfOrExtend(result, ko.observableArray['fn']);
    return result.extend({'trackArrayChanges':true});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.pureComputed"></a>[function <span class="apidocSignatureSpan">knockout.</span>pureComputed (evaluatorFunctionOrOptions, evaluatorFunctionTarget)](#apidoc.element.knockout.pureComputed)
- description and source-code
```javascript
pureComputed = function (evaluatorFunctionOrOptions, evaluatorFunctionTarget) {
    if (typeof evaluatorFunctionOrOptions === 'function') {
        return ko.computed(evaluatorFunctionOrOptions, evaluatorFunctionTarget, {'pure':true});
    } else {
        evaluatorFunctionOrOptions = ko.utils.extend({}, evaluatorFunctionOrOptions);   // make a copy of the parameter object
        evaluatorFunctionOrOptions['pure'] = true;
        return ko.computed(evaluatorFunctionOrOptions, evaluatorFunctionTarget);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.removeNode"></a>[function <span class="apidocSignatureSpan">knockout.</span>removeNode (node)](#apidoc.element.knockout.removeNode)
- description and source-code
```javascript
removeNode = function (node) {
    ko.cleanNode(node);
    if (node.parentNode)
        node.parentNode.removeChild(node);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.renderTemplate"></a>[function <span class="apidocSignatureSpan">knockout.</span>renderTemplate (template, dataOrBindingContext, options, targetNodeOrNodeArray, renderMode)](#apidoc.element.knockout.renderTemplate)
- description and source-code
```javascript
renderTemplate = function (template, dataOrBindingContext, options, targetNodeOrNodeArray, renderMode) {
    options = options || {};
    if ((options['templateEngine'] || _templateEngine) == undefined)
        throw new Error("Set a template engine before calling renderTemplate");
    renderMode = renderMode || "replaceChildren";

    if (targetNodeOrNodeArray) {
        var firstTargetNode = getFirstNodeFromPossibleArray(targetNodeOrNodeArray);

        var whenToDispose = function () { return (!firstTargetNode) || !ko.utils.domNodeIsAttachedToDocument(firstTargetNode); }; //
Passive disposal (on next evaluation)
        var activelyDisposeWhenNodeIsRemoved = (firstTargetNode && renderMode == "replaceNode") ? firstTargetNode.parentNode : firstTargetNode
;

        return ko.dependentObservable( // So the DOM is automatically updated when any dependency changes
            function () {
                // Ensure we've got a proper binding context to work with
                var bindingContext = (dataOrBindingContext && (dataOrBindingContext instanceof ko.bindingContext))
                    ? dataOrBindingContext
                    : new ko.bindingContext(dataOrBindingContext, null, null, null, { "exportDependencies": true });

                var templateName = resolveTemplateName(template, bindingContext['$data'], bindingContext),
                    renderedNodesArray = executeTemplate(targetNodeOrNodeArray, renderMode, templateName, bindingContext, options
);

                if (renderMode == "replaceNode") {
                    targetNodeOrNodeArray = renderedNodesArray;
                    firstTargetNode = getFirstNodeFromPossibleArray(targetNodeOrNodeArray);
                }
            },
            null,
            { disposeWhen: whenToDispose, disposeWhenNodeIsRemoved: activelyDisposeWhenNodeIsRemoved }
        );
    } else {
        // We don't yet have a DOM node to evaluate, so use a memo and render the template later when there is a DOM node
        return ko.memoization.memoize(function (domNode) {
            ko.renderTemplate(template, dataOrBindingContext, options, domNode, "replaceNode");
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.renderTemplateForEach"></a>[function <span class="apidocSignatureSpan">knockout.</span>renderTemplateForEach (template, arrayOrObservableArray, options, targetNode, parentBindingContext)](#apidoc.element.knockout.renderTemplateForEach)
- description and source-code
```javascript
renderTemplateForEach = function (template, arrayOrObservableArray, options, targetNode, parentBindingContext) {
    // Since setDomNodeChildrenFromArrayMapping always calls executeTemplateForArrayItem and then
    // activateBindingsCallback for added items, we can store the binding context in the former to use in the latter.
    var arrayItemContext;

    // This will be called by setDomNodeChildrenFromArrayMapping to get the nodes to add to targetNode
    var executeTemplateForArrayItem = function (arrayValue, index) {
        // Support selecting template as a function of the data being rendered
        arrayItemContext = parentBindingContext['createChildContext'](arrayValue, options['as'], function(context) {
            context['$index'] = index;
        });

        var templateName = resolveTemplateName(template, arrayValue, arrayItemContext);
        return executeTemplate(null, "ignoreTargetNode", templateName, arrayItemContext, options);
    }

    // This will be called whenever setDomNodeChildrenFromArrayMapping has added nodes to targetNode
    var activateBindingsCallback = function(arrayValue, addedNodesArray, index) {
        activateBindingsOnContinuousNodeArray(addedNodesArray, arrayItemContext);
        if (options['afterRender'])
            options['afterRender'](addedNodesArray, arrayValue);

        // release the "cache" variable, so that it can be collected by
        // the GC when its value isn't used from within the bindings anymore.
        arrayItemContext = null;
    };

    return ko.dependentObservable(function () {
        var unwrappedArray = ko.utils.unwrapObservable(arrayOrObservableArray) || [];
        if (typeof unwrappedArray.length == "undefined") // Coerce single value into array
            unwrappedArray = [unwrappedArray];

        // Filter out any entries marked as destroyed
        var filteredArray = ko.utils.arrayFilter(unwrappedArray, function(item) {
            return options['includeDestroyed'] || item === undefined || item === null || !ko.utils.unwrapObservable(item['_destroy
']);
        });

        // Call setDomNodeChildrenFromArrayMapping, ignoring any observables unwrapped within (most likely from a callback function
).
        // If the array items are observables, though, they will be unwrapped in executeTemplateForArrayItem and managed within
setDomNodeChildrenFromArrayMapping.
        ko.dependencyDetection.ignore(ko.utils.setDomNodeChildrenFromArrayMapping, null, [targetNode, filteredArray, executeTemplateForArrayItem
, options, activateBindingsCallback]);

    }, null, { disposeWhenNodeIsRemoved: targetNode });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.setTemplateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>setTemplateEngine (templateEngine)](#apidoc.element.knockout.setTemplateEngine)
- description and source-code
```javascript
setTemplateEngine = function (templateEngine) {
    if ((templateEngine != undefined) && !(templateEngine instanceof ko.templateEngine))
        throw new Error("templateEngine must inherit from ko.templateEngine");
    _templateEngine = templateEngine;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.storedBindingContextForNode"></a>[function <span class="apidocSignatureSpan">knockout.</span>storedBindingContextForNode (node, bindingContext)](#apidoc.element.knockout.storedBindingContextForNode)
- description and source-code
```javascript
storedBindingContextForNode = function (node, bindingContext) {
    if (arguments.length == 2) {
        ko.utils.domData.set(node, storedBindingContextDomDataKey, bindingContext);
        if (bindingContext._subscribable)
            bindingContext._subscribable._addNode(node);
    } else {
        return ko.utils.domData.get(node, storedBindingContextDomDataKey);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.subscribable"></a>[function <span class="apidocSignatureSpan">knockout.</span>subscribable ()](#apidoc.element.knockout.subscribable)
- description and source-code
```javascript
subscribable = function () {
    ko.utils.setPrototypeOfOrExtend(this, ko_subscribable_fn);
    ko_subscribable_fn.init(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.subscription"></a>[function <span class="apidocSignatureSpan">knockout.</span>subscription (target, callback, disposeCallback)](#apidoc.element.knockout.subscription)
- description and source-code
```javascript
subscription = function (target, callback, disposeCallback) {
    this._target = target;
    this.callback = callback;
    this.disposeCallback = disposeCallback;
    this.isDisposed = false;
    ko.exportProperty(this, 'dispose', this.dispose);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>templateEngine ()](#apidoc.element.knockout.templateEngine)
- description and source-code
```javascript
templateEngine = function () { }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateSources.anonymousTemplate"></a>[function <span class="apidocSignatureSpan">knockout.</span>templateSources.anonymousTemplate (element)](#apidoc.element.knockout.templateSources.anonymousTemplate)
- description and source-code
```javascript
templateSources.anonymousTemplate = function (element) {
    this.domElement = element;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateSources.domElement"></a>[function <span class="apidocSignatureSpan">knockout.</span>templateSources.domElement (element)](#apidoc.element.knockout.templateSources.domElement)
- description and source-code
```javascript
templateSources.domElement = function (element) {
    this.domElement = element;

    if (element) {
        var tagNameLower = ko.utils.tagNameLower(element);
        this.templateType =
            tagNameLower === "script" ? templateScript :
            tagNameLower === "textarea" ? templateTextArea :
                // For browsers with proper <template> element support, where the .content property gives a document fragment
            tagNameLower == "template" && element.content && element.content.nodeType === 11 ? templateTemplate :
            templateElement;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.toJS"></a>[function <span class="apidocSignatureSpan">knockout.</span>toJS (rootObject)](#apidoc.element.knockout.toJS)
- description and source-code
```javascript
toJS = function (rootObject) {
    if (arguments.length == 0)
        throw new Error("When calling ko.toJS, pass the object you want to convert.");

    // We just unwrap everything at every level in the object graph
    return mapJsObjectGraph(rootObject, function(valueToMap) {
        // Loop because an observable's value might in turn be another observable wrapper
        for (var i = 0; ko.isObservable(valueToMap) && (i < maxNestedObservableDepth); i++)
            valueToMap = valueToMap();
        return valueToMap;
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.toJSON"></a>[function <span class="apidocSignatureSpan">knockout.</span>toJSON (rootObject, replacer, space)](#apidoc.element.knockout.toJSON)
- description and source-code
```javascript
toJSON = function (rootObject, replacer, space) {     // replacer and space are optional
    var plainJavaScriptObject = ko.toJS(rootObject);
    return ko.utils.stringifyJson(plainJavaScriptObject, replacer, space);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.unwrap"></a>[function <span class="apidocSignatureSpan">knockout.</span>unwrap (value)](#apidoc.element.knockout.unwrap)
- description and source-code
```javascript
unwrap = function (value) {
    return ko.isObservable(value) ? value() : value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.bindingContext"></a>[module knockout.bindingContext](#apidoc.module.knockout.bindingContext)

#### <a name="apidoc.element.knockout.bindingContext.bindingContext"></a>[function <span class="apidocSignatureSpan">knockout.</span>bindingContext (dataItemOrAccessor, parentContext, dataItemAlias, extendCallback, options)](#apidoc.element.knockout.bindingContext.bindingContext)
- description and source-code
```javascript
bindingContext = function (dataItemOrAccessor, parentContext, dataItemAlias, extendCallback, options) {

    // The binding context object includes static properties for the current, parent, and root view models.
    // If a view model is actually stored in an observable, the corresponding binding context object, and
    // any child contexts, must be updated when the view model is changed.
    function updateContext() {
        // Most of the time, the context will directly get a view model object, but if a function is given,
        // we call the function to retrieve the view model. If the function accesses any observables or returns
        // an observable, the dependency is tracked, and those observables can later cause the binding
        // context to be updated.
        var dataItemOrObservable = isFunc ? dataItemOrAccessor() : dataItemOrAccessor,
            dataItem = ko.utils.unwrapObservable(dataItemOrObservable);

        if (parentContext) {
            // When a "parent" context is given, register a dependency on the parent context. Thus whenever the
            // parent context is updated, this context will also be updated.
            if (parentContext._subscribable)
                parentContext._subscribable();

            // Copy $root and any custom properties from the parent context
            ko.utils.extend(self, parentContext);

            // Because the above copy overwrites our own properties, we need to reset them.
            self._subscribable = subscribable;
        } else {
            self['$parents'] = [];
            self['$root'] = dataItem;

            // Export 'ko' in the binding context so it will be available in bindings and templates
            // even if 'ko' isn't exported as a global, such as when using an AMD loader.
            // See https://github.com/SteveSanderson/knockout/issues/490
            self['ko'] = ko;
        }
        self['$rawData'] = dataItemOrObservable;
        self['$data'] = dataItem;
        if (dataItemAlias)
            self[dataItemAlias] = dataItem;

        // The extendCallback function is provided when creating a child context or extending a context.
        // It handles the specific actions needed to finish setting up the binding context. Actions in this
        // function could also add dependencies to this binding context.
        if (extendCallback)
            extendCallback(self, parentContext, dataItem);

        return self['$data'];
    }
    function disposeWhen() {
        return nodes && !ko.utils.anyDomNodeIsAttachedToDocument(nodes);
    }

    var self = this,
        isFunc = typeof(dataItemOrAccessor) == "function" && !ko.isObservable(dataItemOrAccessor),
        nodes,
        subscribable;

    if (options && options['exportDependencies']) {
        // The "exportDependencies" option means that the calling code will track any dependencies and re-create
        // the binding context when they change.
        updateContext();
    } else {
        subscribable = ko.dependentObservable(updateContext, null, { disposeWhen: disposeWhen, disposeWhenNodeIsRemoved: true });

        // At this point, the binding context has been initialized, and the "subscribable" computed observable is
        // subscribed to any observables that were accessed in the process. If there is nothing to track, the
        // computed will be inactive, and we can safely throw it away. If it's active, the computed is stored in
        // the context object.
        if (subscribable.isActive()) {
            self._subscribable = subscribable;

            // Always notify because even if the model ($data) hasn't changed, other context properties might have changed
            subscribable['equalityComparer'] = null;

            // We need to be able to dispose of this computed observable when it's no longer needed. This would be
            // easy if we had a single node to watch, but binding contexts can be used by many different nodes, and
            // we cannot assume that those nodes have any relation to each other. So instead we track any node that ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.bindingContext.prototype"></a>[module knockout.bindingContext.prototype](#apidoc.module.knockout.bindingContext.prototype)

#### <a name="apidoc.element.knockout.bindingContext.prototype.createChildContext"></a>[function <span class="apidocSignatureSpan">knockout.bindingContext.prototype.</span>createChildContext (dataItemOrAccessor, dataItemAlias, extendCallback, options)](#apidoc.element.knockout.bindingContext.prototype.createChildContext)
- description and source-code
```javascript
createChildContext = function (dataItemOrAccessor, dataItemAlias, extendCallback, options) {
    return new ko.bindingContext(dataItemOrAccessor, this, dataItemAlias, function(self, parentContext) {
        // Extend the context hierarchy by setting the appropriate pointers
        self['$parentContext'] = parentContext;
        self['$parent'] = parentContext['$data'];
        self['$parents'] = (parentContext['$parents'] || []).slice(0);
        self['$parents'].unshift(self['$parent']);
        if (extendCallback)
            extendCallback(self);
    }, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingContext.prototype.createStaticChildContext"></a>[function <span class="apidocSignatureSpan">knockout.bindingContext.prototype.</span>createStaticChildContext (dataItemOrAccessor, dataItemAlias)](#apidoc.element.knockout.bindingContext.prototype.createStaticChildContext)
- description and source-code
```javascript
createStaticChildContext = function (dataItemOrAccessor, dataItemAlias) {
    return this['createChildContext'](dataItemOrAccessor, dataItemAlias, null, { "exportDependencies": true });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingContext.prototype.extend"></a>[function <span class="apidocSignatureSpan">knockout.bindingContext.prototype.</span>extend (properties)](#apidoc.element.knockout.bindingContext.prototype.extend)
- description and source-code
```javascript
extend = function (properties) {
    // If the parent context references an observable view model, "_subscribable" will always be the
    // latest view model object. If not, "_subscribable" isn't set, and we can use the static "$data" value.
    return new ko.bindingContext(this._subscribable || this['$data'], this, null, function(self, parentContext) {
        // This "child" context doesn't directly track a parent observable view model,
        // so we need to manually set the $rawData value to match the parent.
        self['$rawData'] = parentContext['$rawData'];
        ko.utils.extend(self, typeof(properties) == "function" ? properties() : properties);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.bindingProvider"></a>[module knockout.bindingProvider](#apidoc.module.knockout.bindingProvider)

#### <a name="apidoc.element.knockout.bindingProvider.bindingProvider"></a>[function <span class="apidocSignatureSpan">knockout.</span>bindingProvider ()](#apidoc.element.knockout.bindingProvider.bindingProvider)
- description and source-code
```javascript
bindingProvider = function () {
    this.bindingCache = {};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.bindingProvider.prototype"></a>[module knockout.bindingProvider.prototype](#apidoc.module.knockout.bindingProvider.prototype)

#### <a name="apidoc.element.knockout.bindingProvider.prototype.getBindingAccessors"></a>[function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>getBindingAccessors (node, bindingContext)](#apidoc.element.knockout.bindingProvider.prototype.getBindingAccessors)
- description and source-code
```javascript
getBindingAccessors = function (node, bindingContext) {
    var bindingsString = this['getBindingsString'](node, bindingContext),
        parsedBindings = bindingsString ? this['parseBindingsString'](bindingsString, bindingContext, node, { 'valueAccessors':
true }) : null;
    return ko.components.addBindingsForCustomElement(parsedBindings, node, bindingContext, /* valueAccessors */ true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingProvider.prototype.getBindings"></a>[function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>getBindings (node, bindingContext)](#apidoc.element.knockout.bindingProvider.prototype.getBindings)
- description and source-code
```javascript
getBindings = function (node, bindingContext) {
    var bindingsString = this['getBindingsString'](node, bindingContext),
        parsedBindings = bindingsString ? this['parseBindingsString'](bindingsString, bindingContext, node) : null;
    return ko.components.addBindingsForCustomElement(parsedBindings, node, bindingContext, /* valueAccessors */ false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingProvider.prototype.getBindingsString"></a>[function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>getBindingsString (node, bindingContext)](#apidoc.element.knockout.bindingProvider.prototype.getBindingsString)
- description and source-code
```javascript
getBindingsString = function (node, bindingContext) {
    switch (node.nodeType) {
        case 1: return node.getAttribute(defaultBindingAttributeName);   // Element
        case 8: return ko.virtualElements.virtualNodeBindingValue(node); // Comment node
        default: return null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingProvider.prototype.nodeHasBindings"></a>[function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>nodeHasBindings (node)](#apidoc.element.knockout.bindingProvider.prototype.nodeHasBindings)
- description and source-code
```javascript
nodeHasBindings = function (node) {
    switch (node.nodeType) {
        case 1: // Element
            return node.getAttribute(defaultBindingAttributeName) != null
                || ko.components['getComponentNameForNode'](node);
        case 8: // Comment node
            return ko.virtualElements.hasBindingValue(node);
        default: return false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.bindingProvider.prototype.parseBindingsString"></a>[function <span class="apidocSignatureSpan">knockout.bindingProvider.prototype.</span>parseBindingsString (bindingsString, bindingContext, node, options)](#apidoc.element.knockout.bindingProvider.prototype.parseBindingsString)
- description and source-code
```javascript
parseBindingsString = function (bindingsString, bindingContext, node, options) {
    try {
        var bindingFunction = createBindingsStringEvaluatorViaCache(bindingsString, this.bindingCache, options);
        return bindingFunction(bindingContext, node);
    } catch (ex) {
        ex.message = "Unable to parse bindings.\nBindings value: " + bindingsString + "\nMessage: " + ex.message;
        throw ex;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.components"></a>[module knockout.components](#apidoc.module.knockout.components)

#### <a name="apidoc.element.knockout.components._getFirstResultFromLoaders"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>_getFirstResultFromLoaders (methodName, argsExceptCallback, callback, candidateLoaders)](#apidoc.element.knockout.components._getFirstResultFromLoaders)
- description and source-code
```javascript
function getFirstResultFromLoaders(methodName, argsExceptCallback, callback, candidateLoaders) {
    // On the first call in the stack, start with the full set of loaders
    if (!candidateLoaders) {
        candidateLoaders = ko.components['loaders'].slice(0); // Use a copy, because we'll be mutating this array
    }

    // Try the next candidate
    var currentCandidateLoader = candidateLoaders.shift();
    if (currentCandidateLoader) {
        var methodInstance = currentCandidateLoader[methodName];
        if (methodInstance) {
            var wasAborted = false,
                synchronousReturnValue = methodInstance.apply(currentCandidateLoader, argsExceptCallback.concat(function(result) {
                    if (wasAborted) {
                        callback(null);
                    } else if (result !== null) {
                        // This candidate returned a value. Use it.
                        callback(result);
                    } else {
                        // Try the next candidate
                        getFirstResultFromLoaders(methodName, argsExceptCallback, callback, candidateLoaders);
                    }
                }));

            // Currently, loaders may not return anything synchronously. This leaves open the possibility
            // that we'll extend the API to support synchronous return values in the future. It won't be
            // a breaking change, because currently no loader is allowed to return anything except undefined.
            if (synchronousReturnValue !== undefined) {
                wasAborted = true;

                // Method to suppress exceptions will remain undocumented. This is only to keep
                // KO's specs running tidily, since we can observe the loading got aborted without
                // having exceptions cluttering up the console too.
                if (!currentCandidateLoader['suppressLoaderExceptions']) {
                    throw new Error('Component loaders must supply values by invoking the callback, not by returning values synchronously
.');
                }
            }
        } else {
            // This candidate doesn't have the relevant handler. Synchronously move on to the next one.
            getFirstResultFromLoaders(methodName, argsExceptCallback, callback, candidateLoaders);
        }
    } else {
        // No candidates returned a value
        callback(null);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.addBindingsForCustomElement"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>addBindingsForCustomElement (allBindings, node, bindingContext, valueAccessors)](#apidoc.element.knockout.components.addBindingsForCustomElement)
- description and source-code
```javascript
addBindingsForCustomElement = function (allBindings, node, bindingContext, valueAccessors) {
    // Determine if it's really a custom element matching a component
    if (node.nodeType === 1) {
        var componentName = ko.components['getComponentNameForNode'](node);
        if (componentName) {
            // It does represent a component, so add a component binding for it
            allBindings = allBindings || {};

            if (allBindings['component']) {
                // Avoid silently overwriting some other 'component' binding that may already be on the element
                throw new Error('Cannot use the "component" binding on a custom element matching a component');
            }

            var componentBindingValue = { 'name': componentName, 'params': getComponentParamsFromCustomElement(node, bindingContext
) };

            allBindings['component'] = valueAccessors
                ? function() { return componentBindingValue; }
                : componentBindingValue;
        }
    }

    return allBindings;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.clearCachedDefinition"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>clearCachedDefinition (componentName)](#apidoc.element.knockout.components.clearCachedDefinition)
- description and source-code
```javascript
clearCachedDefinition = function (componentName) {
    delete loadedDefinitionsCache[componentName];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.get"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>get (componentName, callback)](#apidoc.element.knockout.components.get)
- description and source-code
```javascript
get = function (componentName, callback) {
    var cachedDefinition = getObjectOwnProperty(loadedDefinitionsCache, componentName);
    if (cachedDefinition) {
        // It's already loaded and cached. Reuse the same definition object.
        // Note that for API consistency, even cache hits complete asynchronously by default.
        // You can bypass this by putting synchronous:true on your component config.
        if (cachedDefinition.isSynchronousComponent) {
            ko.dependencyDetection.ignore(function() { // See comment in loaderRegistryBehaviors.js for reasoning
                callback(cachedDefinition.definition);
            });
        } else {
            ko.tasks.schedule(function() { callback(cachedDefinition.definition); });
        }
    } else {
        // Join the loading process that is already underway, or start a new one.
        loadComponentAndNotify(componentName, callback);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.getComponentNameForNode"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>getComponentNameForNode (node)](#apidoc.element.knockout.components.getComponentNameForNode)
- description and source-code
```javascript
getComponentNameForNode = function (node) {
    var tagNameLower = ko.utils.tagNameLower(node);
    if (ko.components.isRegistered(tagNameLower)) {
        // Try to determine that this node can be considered a *custom* element; see https://github.com/knockout/knockout/issues
/1603
        if (tagNameLower.indexOf('-') != -1 || ('' + node) == "[object HTMLUnknownElement]" || (ko.utils.ieVersion <= 8 && node.
tagName === tagNameLower)) {
            return tagNameLower;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.isRegistered"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>isRegistered (componentName)](#apidoc.element.knockout.components.isRegistered)
- description and source-code
```javascript
isRegistered = function (componentName) {
    return defaultConfigRegistry.hasOwnProperty(componentName);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.register"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>register (componentName, config)](#apidoc.element.knockout.components.register)
- description and source-code
```javascript
register = function (componentName, config) {
    if (!config) {
        throw new Error('Invalid configuration for ' + componentName);
    }

    if (ko.components.isRegistered(componentName)) {
        throw new Error('Component ' + componentName + ' is already registered');
    }

    defaultConfigRegistry[componentName] = config;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.unregister"></a>[function <span class="apidocSignatureSpan">knockout.components.</span>unregister (componentName)](#apidoc.element.knockout.components.unregister)
- description and source-code
```javascript
unregister = function (componentName) {
    delete defaultConfigRegistry[componentName];
    ko.components.clearCachedDefinition(componentName);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.components.defaultLoader"></a>[module knockout.components.defaultLoader](#apidoc.module.knockout.components.defaultLoader)

#### <a name="apidoc.element.knockout.components.defaultLoader.getConfig"></a>[function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>getConfig (componentName, callback)](#apidoc.element.knockout.components.defaultLoader.getConfig)
- description and source-code
```javascript
getConfig = function (componentName, callback) {
    var result = defaultConfigRegistry.hasOwnProperty(componentName)
        ? defaultConfigRegistry[componentName]
        : null;
    callback(result);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.defaultLoader.loadComponent"></a>[function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>loadComponent (componentName, config, callback)](#apidoc.element.knockout.components.defaultLoader.loadComponent)
- description and source-code
```javascript
loadComponent = function (componentName, config, callback) {
    var errorCallback = makeErrorCallback(componentName);
    possiblyGetConfigFromAmd(errorCallback, config, function(loadedConfig) {
        resolveConfig(componentName, errorCallback, loadedConfig, callback);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.defaultLoader.loadTemplate"></a>[function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>loadTemplate (componentName, templateConfig, callback)](#apidoc.element.knockout.components.defaultLoader.loadTemplate)
- description and source-code
```javascript
loadTemplate = function (componentName, templateConfig, callback) {
    resolveTemplate(makeErrorCallback(componentName), templateConfig, callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.components.defaultLoader.loadViewModel"></a>[function <span class="apidocSignatureSpan">knockout.components.defaultLoader.</span>loadViewModel (componentName, viewModelConfig, callback)](#apidoc.element.knockout.components.defaultLoader.loadViewModel)
- description and source-code
```javascript
loadViewModel = function (componentName, viewModelConfig, callback) {
    resolveViewModel(makeErrorCallback(componentName), viewModelConfig, callback);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.dependencyDetection"></a>[module knockout.dependencyDetection](#apidoc.module.knockout.dependencyDetection)

#### <a name="apidoc.element.knockout.dependencyDetection.begin"></a>[function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>begin (options)](#apidoc.element.knockout.dependencyDetection.begin)
- description and source-code
```javascript
function begin(options) {
    outerFrames.push(currentFrame);
    currentFrame = options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependencyDetection.end"></a>[function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>end ()](#apidoc.element.knockout.dependencyDetection.end)
- description and source-code
```javascript
function end() {
    currentFrame = outerFrames.pop();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependencyDetection.getDependenciesCount"></a>[function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>getDependenciesCount ()](#apidoc.element.knockout.dependencyDetection.getDependenciesCount)
- description and source-code
```javascript
getDependenciesCount = function () {
    if (currentFrame)
        return currentFrame.computed.getDependenciesCount();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependencyDetection.ignore"></a>[function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>ignore (callback, callbackTarget, callbackArgs)](#apidoc.element.knockout.dependencyDetection.ignore)
- description and source-code
```javascript
ignore = function (callback, callbackTarget, callbackArgs) {
    try {
        begin();
        return callback.apply(callbackTarget, callbackArgs || []);
    } finally {
        end();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependencyDetection.isInitial"></a>[function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>isInitial ()](#apidoc.element.knockout.dependencyDetection.isInitial)
- description and source-code
```javascript
isInitial = function () {
    if (currentFrame)
        return currentFrame.isInitial;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependencyDetection.registerDependency"></a>[function <span class="apidocSignatureSpan">knockout.dependencyDetection.</span>registerDependency (subscribable)](#apidoc.element.knockout.dependencyDetection.registerDependency)
- description and source-code
```javascript
registerDependency = function (subscribable) {
    if (currentFrame) {
        if (!ko.isSubscribable(subscribable))
            throw new Error("Only subscribable things can act as dependencies");
        currentFrame.callback.call(currentFrame.callbackTarget, subscribable, subscribable._id || (subscribable._id = getId()));
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.dependentObservable"></a>[module knockout.dependentObservable](#apidoc.module.knockout.dependentObservable)

#### <a name="apidoc.element.knockout.dependentObservable.dependentObservable"></a>[function <span class="apidocSignatureSpan">knockout.</span>dependentObservable (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.dependentObservable.dependentObservable)
- description and source-code
```javascript
dependentObservable = function (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options) {
    if (typeof evaluatorFunctionOrOptions === "object") {
        // Single-parameter syntax - everything is on this "options" param
        options = evaluatorFunctionOrOptions;
    } else {
        // Multi-parameter syntax - construct the options according to the params passed
        options = options || {};
        if (evaluatorFunctionOrOptions) {
            options["read"] = evaluatorFunctionOrOptions;
        }
    }
    if (typeof options["read"] != "function")
        throw Error("Pass a function that returns the value of the ko.computed");

    var writeFunction = options["write"];
    var state = {
        latestValue: undefined,
        isStale: true,
        isDirty: true,
        isBeingEvaluated: false,
        suppressDisposalUntilDisposeWhenReturnsFalse: false,
        isDisposed: false,
        pure: false,
        isSleeping: false,
        readFunction: options["read"],
        evaluatorFunctionTarget: evaluatorFunctionTarget || options["owner"],
        disposeWhenNodeIsRemoved: options["disposeWhenNodeIsRemoved"] || options.disposeWhenNodeIsRemoved || null,
        disposeWhen: options["disposeWhen"] || options.disposeWhen,
        domNodeDisposalCallback: null,
        dependencyTracking: {},
        dependenciesCount: 0,
        evaluationTimeoutInstance: null
    };

    function computedObservable() {
        if (arguments.length > 0) {
            if (typeof writeFunction === "function") {
                // Writing a value
                writeFunction.apply(state.evaluatorFunctionTarget, arguments);
            } else {
                throw new Error("Cannot write a value to a ko.computed unless you specify a 'write' option. If you wish to read
the current value, don't pass any parameters.");
            }
            return this; // Permits chained assignments
        } else {
            // Reading the value
            ko.dependencyDetection.registerDependency(computedObservable);
            if (state.isDirty || (state.isSleeping && computedObservable.haveDependenciesChanged())) {
                computedObservable.evaluateImmediate();
            }
            return state.latestValue;
        }
    }

    computedObservable[computedState] = state;
    computedObservable.hasWriteFunction = typeof writeFunction === "function";

    // Inherit from 'subscribable'
    if (!ko.utils.canSetPrototype) {
        // 'subscribable' won't be on the prototype chain unless we put it there directly
        ko.utils.extend(computedObservable, ko.subscribable['fn']);
    }
    ko.subscribable['fn'].init(computedObservable);

    // Inherit from 'computed'
    ko.utils.setPrototypeOfOrExtend(computedObservable, computedFn);

    if (options['pure']) {
        state.pure = true;
        state.isSleeping = true;     // Starts off sleeping; will awake on the first subscription
        ko.utils.extend(computedObservable, pureComputedOverrides);
    } else if (options['deferEvaluation']) {
        ko.utils.extend(computedObservable, deferEvaluationOverrides);
    }

    if (ko.options['deferUpdates']) {
        ko.extenders['deferred'](computedObservable, true);
    }

    if (DEBUG) {
        // #1731 - Aid debugging by exposing the computed's options
        computedObservable["_options"] = options;
    }

    if (state.disposeWhenNodeIsRemoved) {
        // Since this computed is associated with a DOM node, and we don't want to dispose the computed
        // until the DOM node is *removed* from the document (as opposed to never having been in the document),
        // we'll prevent disposal until "disposeWhen" first returns false.
        state.suppressDisposalUntilDisposeWhenReturnsFalse = true;

        // disposeWhenNodeIsRemoved: true can be used to opt into the "only dispose after first false result"
        // behaviour even if there's no specific node to watch. In that case, clear the option so we don't try
        // to watch for a non-node's disposal. This technique is intended for KO's internal use only and shouldn't ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.__ko_proto__"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.</span>__ko_proto__ (initialValue)](#apidoc.element.knockout.dependentObservable.__ko_proto__)
- description and source-code
```javascript
__ko_proto__ = function (initialValue) {
    function observable() {
        if (arguments.length > 0) {
            // Write

            // Ignore writes if the value hasn't changed
            if (observable.isDifferent(observable[observableLatestValue], arguments[0])) {
                observable.valueWillMutate();
                observable[observableLatestValue] = arguments[0];
                observable.valueHasMutated();
            }
            return this; // Permits chained assignments
        }
        else {
            // Read
            ko.dependencyDetection.registerDependency(observable); // The caller only needs to be notified of changes if they did
 a "read" operation
            return observable[observableLatestValue];
        }
    }

    observable[observableLatestValue] = initialValue;

    // Inherit from 'subscribable'
    if (!ko.utils.canSetPrototype) {
        // 'subscribable' won't be on the prototype chain unless we put it there directly
        ko.utils.extend(observable, ko.subscribable['fn']);
    }
    ko.subscribable['fn'].init(observable);

    // Inherit from 'observable'
    ko.utils.setPrototypeOfOrExtend(observable, observableFn);

    if (ko.options['deferUpdates']) {
        ko.extenders['deferred'](observable, true);
    }

    return observable;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.dependentObservable.fn"></a>[module knockout.dependentObservable.fn](#apidoc.module.knockout.dependentObservable.fn)

#### <a name="apidoc.element.knockout.dependentObservable.fn.__ko_proto__"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>__ko_proto__ (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options)](#apidoc.element.knockout.dependentObservable.fn.__ko_proto__)
- description and source-code
```javascript
__ko_proto__ = function (evaluatorFunctionOrOptions, evaluatorFunctionTarget, options) {
    if (typeof evaluatorFunctionOrOptions === "object") {
        // Single-parameter syntax - everything is on this "options" param
        options = evaluatorFunctionOrOptions;
    } else {
        // Multi-parameter syntax - construct the options according to the params passed
        options = options || {};
        if (evaluatorFunctionOrOptions) {
            options["read"] = evaluatorFunctionOrOptions;
        }
    }
    if (typeof options["read"] != "function")
        throw Error("Pass a function that returns the value of the ko.computed");

    var writeFunction = options["write"];
    var state = {
        latestValue: undefined,
        isStale: true,
        isDirty: true,
        isBeingEvaluated: false,
        suppressDisposalUntilDisposeWhenReturnsFalse: false,
        isDisposed: false,
        pure: false,
        isSleeping: false,
        readFunction: options["read"],
        evaluatorFunctionTarget: evaluatorFunctionTarget || options["owner"],
        disposeWhenNodeIsRemoved: options["disposeWhenNodeIsRemoved"] || options.disposeWhenNodeIsRemoved || null,
        disposeWhen: options["disposeWhen"] || options.disposeWhen,
        domNodeDisposalCallback: null,
        dependencyTracking: {},
        dependenciesCount: 0,
        evaluationTimeoutInstance: null
    };

    function computedObservable() {
        if (arguments.length > 0) {
            if (typeof writeFunction === "function") {
                // Writing a value
                writeFunction.apply(state.evaluatorFunctionTarget, arguments);
            } else {
                throw new Error("Cannot write a value to a ko.computed unless you specify a 'write' option. If you wish to read
the current value, don't pass any parameters.");
            }
            return this; // Permits chained assignments
        } else {
            // Reading the value
            ko.dependencyDetection.registerDependency(computedObservable);
            if (state.isDirty || (state.isSleeping && computedObservable.haveDependenciesChanged())) {
                computedObservable.evaluateImmediate();
            }
            return state.latestValue;
        }
    }

    computedObservable[computedState] = state;
    computedObservable.hasWriteFunction = typeof writeFunction === "function";

    // Inherit from 'subscribable'
    if (!ko.utils.canSetPrototype) {
        // 'subscribable' won't be on the prototype chain unless we put it there directly
        ko.utils.extend(computedObservable, ko.subscribable['fn']);
    }
    ko.subscribable['fn'].init(computedObservable);

    // Inherit from 'computed'
    ko.utils.setPrototypeOfOrExtend(computedObservable, computedFn);

    if (options['pure']) {
        state.pure = true;
        state.isSleeping = true;     // Starts off sleeping; will awake on the first subscription
        ko.utils.extend(computedObservable, pureComputedOverrides);
    } else if (options['deferEvaluation']) {
        ko.utils.extend(computedObservable, deferEvaluationOverrides);
    }

    if (ko.options['deferUpdates']) {
        ko.extenders['deferred'](computedObservable, true);
    }

    if (DEBUG) {
        // #1731 - Aid debugging by exposing the computed's options
        computedObservable["_options"] = options;
    }

    if (state.disposeWhenNodeIsRemoved) {
        // Since this computed is associated with a DOM node, and we don't want to dispose the computed
        // until the DOM node is *removed* from the document (as opposed to never having been in the document),
        // we'll prevent disposal until "disposeWhen" first returns false.
        state.suppressDisposalUntilDisposeWhenReturnsFalse = true;

        // disposeWhenNodeIsRemoved: true can be used to opt into the "only dispose after first false result"
        // behaviour even if there's no specific node to watch. In that case, clear the option so we don't try
        // to watch for a non-node's disposal. This technique is intended for KO's internal use only and shouldn't ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.addDependencyTracking"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>addDependencyTracking (id, target, trackingObj)](#apidoc.element.knockout.dependentObservable.fn.addDependencyTracking)
- description and source-code
```javascript
addDependencyTracking = function (id, target, trackingObj) {
    if (this[computedState].pure && target === this) {
        throw Error("A 'pure' computed must not be called recursively");
    }

    this[computedState].dependencyTracking[id] = trackingObj;
    trackingObj._order = this[computedState].dependenciesCount++;
    trackingObj._version = target.getVersion();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.dispose"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>dispose ()](#apidoc.element.knockout.dependentObservable.fn.dispose)
- description and source-code
```javascript
dispose = function () {
    var state = this[computedState];
    if (!state.isSleeping && state.dependencyTracking) {
        ko.utils.objectForEach(state.dependencyTracking, function (id, dependency) {
            if (dependency.dispose)
                dependency.dispose();
        });
    }
    if (state.disposeWhenNodeIsRemoved && state.domNodeDisposalCallback) {
        ko.utils.domNodeDisposal.removeDisposeCallback(state.disposeWhenNodeIsRemoved, state.domNodeDisposalCallback);
    }
    state.dependencyTracking = null;
    state.dependenciesCount = 0;
    state.isDisposed = true;
    state.isStale = false;
    state.isDirty = false;
    state.isSleeping = false;
    state.disposeWhenNodeIsRemoved = null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.equalityComparer"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>equalityComparer (a, b)](#apidoc.element.knockout.dependentObservable.fn.equalityComparer)
- description and source-code
```javascript
function valuesArePrimitiveAndEqual(a, b) {
    var oldValueIsPrimitive = (a === null) || (typeof(a) in primitiveTypes);
    return oldValueIsPrimitive ? (a === b) : false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.evaluateImmediate"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluateImmediate (notifyChange)](#apidoc.element.knockout.dependentObservable.fn.evaluateImmediate)
- description and source-code
```javascript
evaluateImmediate = function (notifyChange) {
    var computedObservable = this,
        state = computedObservable[computedState],
        disposeWhen = state.disposeWhen,
        changed = false;

    if (state.isBeingEvaluated) {
        // If the evaluation of a ko.computed causes side effects, it's possible that it will trigger its own re-evaluation.
        // This is not desirable (it's hard for a developer to realise a chain of dependencies might cause this, and they almost
        // certainly didn't intend infinite re-evaluations). So, for predictability, we simply prevent ko.computeds from causing
        // their own re-evaluation. Further discussion at https://github.com/SteveSanderson/knockout/pull/387
        return;
    }

    // Do not evaluate (and possibly capture new dependencies) if disposed
    if (state.isDisposed) {
        return;
    }

    if (state.disposeWhenNodeIsRemoved && !ko.utils.domNodeIsAttachedToDocument(state.disposeWhenNodeIsRemoved) || disposeWhen &&
disposeWhen()) {
        // See comment above about suppressDisposalUntilDisposeWhenReturnsFalse
        if (!state.suppressDisposalUntilDisposeWhenReturnsFalse) {
            computedObservable.dispose();
            return;
        }
    } else {
        // It just did return false, so we can stop suppressing now
        state.suppressDisposalUntilDisposeWhenReturnsFalse = false;
    }

    state.isBeingEvaluated = true;
    try {
        changed = this.evaluateImmediate_CallReadWithDependencyDetection(notifyChange);
    } finally {
        state.isBeingEvaluated = false;
    }

    if (!state.dependenciesCount) {
        computedObservable.dispose();
    }

    return changed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.evaluateImmediate_CallReadThenEndDependencyDetection"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluateImmediate_CallReadThenEndDependencyDetection (state, dependencyDetectionContext)](#apidoc.element.knockout.dependentObservable.fn.evaluateImmediate_CallReadThenEndDependencyDetection)
- description and source-code
```javascript
evaluateImmediate_CallReadThenEndDependencyDetection = function (state, dependencyDetectionContext) {
    // This function is really part of the evaluateImmediate_CallReadWithDependencyDetection logic.
    // You'd never call it from anywhere else. Factoring it out means that evaluateImmediate_CallReadWithDependencyDetection
    // can be independent of try/finally blocks, which contributes to saving about 40% off the CPU
    // overhead of computed evaluation (on V8 at least).

    try {
        var readFunction = state.readFunction;
        return state.evaluatorFunctionTarget ? readFunction.call(state.evaluatorFunctionTarget) : readFunction();
    } finally {
        ko.dependencyDetection.end();

        // For each subscription no longer being used, remove it from the active subscriptions list and dispose it
        if (dependencyDetectionContext.disposalCount && !state.isSleeping) {
            ko.utils.objectForEach(dependencyDetectionContext.disposalCandidates, computedDisposeDependencyCallback);
        }

        state.isStale = state.isDirty = false;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.evaluateImmediate_CallReadWithDependencyDetection"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluateImmediate_CallReadWithDependencyDetection (notifyChange)](#apidoc.element.knockout.dependentObservable.fn.evaluateImmediate_CallReadWithDependencyDetection)
- description and source-code
```javascript
evaluateImmediate_CallReadWithDependencyDetection = function (notifyChange) {
    // This function is really just part of the evaluateImmediate logic. You would never call it from anywhere else.
    // Factoring it out into a separate function means it can be independent of the try/catch block in evaluateImmediate,
    // which contributes to saving about 40% off the CPU overhead of computed evaluation (on V8 at least).

    var computedObservable = this,
        state = computedObservable[computedState],
        changed = false;

    // Initially, we assume that none of the subscriptions are still being used (i.e., all are candidates for disposal).
    // Then, during evaluation, we cross off any that are in fact still being used.
    var isInitial = state.pure ? undefined : !state.dependenciesCount,   // If we're evaluating when there are no previous dependencies
, it must be the first time
        dependencyDetectionContext = {
            computedObservable: computedObservable,
            disposalCandidates: state.dependencyTracking,
            disposalCount: state.dependenciesCount
        };

    ko.dependencyDetection.begin({
        callbackTarget: dependencyDetectionContext,
        callback: computedBeginDependencyDetectionCallback,
        computed: computedObservable,
        isInitial: isInitial
    });

    state.dependencyTracking = {};
    state.dependenciesCount = 0;

    var newValue = this.evaluateImmediate_CallReadThenEndDependencyDetection(state, dependencyDetectionContext);

    if (computedObservable.isDifferent(state.latestValue, newValue)) {
        if (!state.isSleeping) {
            computedObservable["notifySubscribers"](state.latestValue, "beforeChange");
        }

        state.latestValue = newValue;
        if (DEBUG) computedObservable._latestValue = newValue;

        if (state.isSleeping) {
            computedObservable.updateVersion();
        } else if (notifyChange) {
            computedObservable["notifySubscribers"](state.latestValue);
        }

        changed = true;
    }

    if (isInitial) {
        computedObservable["notifySubscribers"](state.latestValue, "awake");
    }

    return changed;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.evaluatePossiblyAsync"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>evaluatePossiblyAsync ()](#apidoc.element.knockout.dependentObservable.fn.evaluatePossiblyAsync)
- description and source-code
```javascript
evaluatePossiblyAsync = function () {
    var computedObservable = this,
        throttleEvaluationTimeout = computedObservable['throttleEvaluation'];
    if (throttleEvaluationTimeout && throttleEvaluationTimeout >= 0) {
        clearTimeout(this[computedState].evaluationTimeoutInstance);
        this[computedState].evaluationTimeoutInstance = ko.utils.setTimeout(function () {
            computedObservable.evaluateImmediate(true /*notifyChange*/);
        }, throttleEvaluationTimeout);
    } else if (computedObservable._evalDelayed) {
        computedObservable._evalDelayed(true /*isChange*/);
    } else {
        computedObservable.evaluateImmediate(true /*notifyChange*/);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.getDependenciesCount"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>getDependenciesCount ()](#apidoc.element.knockout.dependentObservable.fn.getDependenciesCount)
- description and source-code
```javascript
getDependenciesCount = function () {
    return this[computedState].dependenciesCount;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.haveDependenciesChanged"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>haveDependenciesChanged ()](#apidoc.element.knockout.dependentObservable.fn.haveDependenciesChanged)
- description and source-code
```javascript
haveDependenciesChanged = function () {
    var id, dependency, dependencyTracking = this[computedState].dependencyTracking;
    for (id in dependencyTracking) {
        if (dependencyTracking.hasOwnProperty(id)) {
            dependency = dependencyTracking[id];
            if ((this._evalDelayed && dependency._target._notificationIsPending) || dependency._target.hasChanged(dependency._version
)) {
                return true;
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.isActive"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>isActive ()](#apidoc.element.knockout.dependentObservable.fn.isActive)
- description and source-code
```javascript
isActive = function () {
    var state = this[computedState];
    return state.isDirty || state.dependenciesCount > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.limit"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>limit (limitFunction)](#apidoc.element.knockout.dependentObservable.fn.limit)
- description and source-code
```javascript
limit = function (limitFunction) {
    // Override the limit function with one that delays evaluation as well
    ko.subscribable['fn'].limit.call(this, limitFunction);
    this._evalIfChanged = function () {
        if (this[computedState].isStale) {
            this.evaluateImmediate();
        } else {
            this[computedState].isDirty = false;
        }
        return this[computedState].latestValue;
    };
    this._evalDelayed = function (isChange) {
        this._limitBeforeChange(this[computedState].latestValue);

        // Mark as dirty
        this[computedState].isDirty = true;
        if (isChange) {
            this[computedState].isStale = true;
        }

        // Pass the observable to the "limit" code, which will evaluate it when
        // it's time to do the notification.
        this._limitChange(this);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.markDirty"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>markDirty ()](#apidoc.element.knockout.dependentObservable.fn.markDirty)
- description and source-code
```javascript
markDirty = function () {
    // Process "dirty" events if we can handle delayed notifications
    if (this._evalDelayed && !this[computedState].isBeingEvaluated) {
        this._evalDelayed(false /*isChange*/);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.peek"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>peek (evaluate)](#apidoc.element.knockout.dependentObservable.fn.peek)
- description and source-code
```javascript
peek = function (evaluate) {
    // By default, peek won't re-evaluate, except while the computed is sleeping or to get the initial value when "deferEvaluation
" is set.
    // Pass in true to evaluate if needed.
    var state = this[computedState];
    if ((state.isDirty && (evaluate || !state.dependenciesCount)) || (state.isSleeping && this.haveDependenciesChanged())) {
        this.evaluateImmediate();
    }
    return state.latestValue;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.respondToChange"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>respondToChange ()](#apidoc.element.knockout.dependentObservable.fn.respondToChange)
- description and source-code
```javascript
respondToChange = function () {
    // Ignore "change" events if we've already scheduled a delayed notification
    if (!this._notificationIsPending) {
        this.evaluatePossiblyAsync();
    } else if (this[computedState].isDirty) {
        this[computedState].isStale = true;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.dependentObservable.fn.subscribeToDependency"></a>[function <span class="apidocSignatureSpan">knockout.dependentObservable.fn.</span>subscribeToDependency (target)](#apidoc.element.knockout.dependentObservable.fn.subscribeToDependency)
- description and source-code
```javascript
subscribeToDependency = function (target) {
    if (target._deferUpdates && !this[computedState].disposeWhenNodeIsRemoved) {
        var dirtySub = target.subscribe(this.markDirty, this, 'dirty'),
            changeSub = target.subscribe(this.respondToChange, this);
        return {
            _target: target,
            dispose: function () {
                dirtySub.dispose();
                changeSub.dispose();
            }
        };
    } else {
        return target.subscribe(this.evaluatePossiblyAsync, this);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.expressionRewriting"></a>[module knockout.expressionRewriting](#apidoc.module.knockout.expressionRewriting)

#### <a name="apidoc.element.knockout.expressionRewriting.insertPropertyAccessorsIntoJson"></a>[function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>insertPropertyAccessorsIntoJson (bindingsStringOrKeyValueArray, bindingOptions)](#apidoc.element.knockout.expressionRewriting.insertPropertyAccessorsIntoJson)
- description and source-code
```javascript
function preProcessBindings(bindingsStringOrKeyValueArray, bindingOptions) {
    bindingOptions = bindingOptions || {};

    function processKeyValue(key, val) {
        var writableVal;
        function callPreprocessHook(obj) {
            return (obj && obj['preprocess']) ? (val = obj['preprocess'](val, key, processKeyValue)) : true;
        }
        if (!bindingParams) {
            if (!callPreprocessHook(ko['getBindingHandler'](key)))
                return;

            if (twoWayBindings[key] && (writableVal = getWriteableValue(val))) {
                // For two-way bindings, provide a write method in case the value
                // isn't a writable observable.
                propertyAccessorResultStrings.push("'" + key + "':function(_z){" + writableVal + "=_z}");
            }
        }
        // Values are wrapped in a function so that each value can be accessed independently
        if (makeValueAccessors) {
            val = 'function(){return ' + val + ' }';
        }
        resultStrings.push("'" + key + "':" + val);
    }

    var resultStrings = [],
        propertyAccessorResultStrings = [],
        makeValueAccessors = bindingOptions['valueAccessors'],
        bindingParams = bindingOptions['bindingParams'],
        keyValueArray = typeof bindingsStringOrKeyValueArray === "string" ?
            parseObjectLiteral(bindingsStringOrKeyValueArray) : bindingsStringOrKeyValueArray;

    ko.utils.arrayForEach(keyValueArray, function(keyValue) {
        processKeyValue(keyValue.key || keyValue['unknown'], keyValue.value);
    });

    if (propertyAccessorResultStrings.length)
        processKeyValue('_ko_property_writers', "{" + propertyAccessorResultStrings.join(",") + " }");

    return resultStrings.join(",");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.expressionRewriting.keyValueArrayContainsKey"></a>[function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>keyValueArrayContainsKey (keyValueArray, key)](#apidoc.element.knockout.expressionRewriting.keyValueArrayContainsKey)
- description and source-code
```javascript
keyValueArrayContainsKey = function (keyValueArray, key) {
    for (var i = 0; i < keyValueArray.length; i++)
        if (keyValueArray[i]['key'] == key)
            return true;
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.expressionRewriting.parseObjectLiteral"></a>[function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>parseObjectLiteral (objectLiteralString)](#apidoc.element.knockout.expressionRewriting.parseObjectLiteral)
- description and source-code
```javascript
function parseObjectLiteral(objectLiteralString) {
    // Trim leading and trailing spaces from the string
    var str = ko.utils.stringTrim(objectLiteralString);

    // Trim braces '{' surrounding the whole object literal
    if (str.charCodeAt(0) === 123) str = str.slice(1, -1);

    // Split into tokens
    var result = [], toks = str.match(bindingToken), key, values = [], depth = 0;

    if (toks) {
        // Append a comma so that we don't need a separate code block to deal with the last item
        toks.push(',');

        for (var i = 0, tok; tok = toks[i]; ++i) {
            var c = tok.charCodeAt(0);
            // A comma signals the end of a key/value pair if depth is zero
            if (c === 44) { // ","
                if (depth <= 0) {
                    result.push((key && values.length) ? {key: key, value: values.join('')} : {'unknown': key || values.join('')});
                    key = depth = 0;
                    values = [];
                    continue;
                }
            // Simply skip the colon that separates the name and value
            } else if (c === 58) { // ":"
                if (!depth && !key && values.length === 1) {
                    key = values.pop();
                    continue;
                }
            // A set of slashes is initially matched as a regular expression, but could be division
            } else if (c === 47 && i && tok.length > 1) {  // "/"
                // Look at the end of the previous token to determine if the slash is actually division
                var match = toks[i-1].match(divisionLookBehind);
                if (match && !keywordRegexLookBehind[match[0]]) {
                    // The slash is actually a division punctuator; re-parse the remainder of the string (not including the slash
)
                    str = str.substr(str.indexOf(tok) + 1);
                    toks = str.match(bindingToken);
                    toks.push(',');
                    i = -1;
                    // Continue with just the slash
                    tok = '/';
                }
            // Increment depth for parentheses, braces, and brackets so that interior commas are ignored
            } else if (c === 40 || c === 123 || c === 91) { // '(', '{', '['
                ++depth;
            } else if (c === 41 || c === 125 || c === 93) { // ')', '}', ']'
                --depth;
            // The key will be the first token; if it's a string, trim the quotes
            } else if (!key && !values.length && (c === 34 || c === 39)) { // '"', "'"
                tok = tok.slice(1, -1);
            }
            values.push(tok);
        }
    }
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.expressionRewriting.preProcessBindings"></a>[function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>preProcessBindings (bindingsStringOrKeyValueArray, bindingOptions)](#apidoc.element.knockout.expressionRewriting.preProcessBindings)
- description and source-code
```javascript
function preProcessBindings(bindingsStringOrKeyValueArray, bindingOptions) {
    bindingOptions = bindingOptions || {};

    function processKeyValue(key, val) {
        var writableVal;
        function callPreprocessHook(obj) {
            return (obj && obj['preprocess']) ? (val = obj['preprocess'](val, key, processKeyValue)) : true;
        }
        if (!bindingParams) {
            if (!callPreprocessHook(ko['getBindingHandler'](key)))
                return;

            if (twoWayBindings[key] && (writableVal = getWriteableValue(val))) {
                // For two-way bindings, provide a write method in case the value
                // isn't a writable observable.
                propertyAccessorResultStrings.push("'" + key + "':function(_z){" + writableVal + "=_z}");
            }
        }
        // Values are wrapped in a function so that each value can be accessed independently
        if (makeValueAccessors) {
            val = 'function(){return ' + val + ' }';
        }
        resultStrings.push("'" + key + "':" + val);
    }

    var resultStrings = [],
        propertyAccessorResultStrings = [],
        makeValueAccessors = bindingOptions['valueAccessors'],
        bindingParams = bindingOptions['bindingParams'],
        keyValueArray = typeof bindingsStringOrKeyValueArray === "string" ?
            parseObjectLiteral(bindingsStringOrKeyValueArray) : bindingsStringOrKeyValueArray;

    ko.utils.arrayForEach(keyValueArray, function(keyValue) {
        processKeyValue(keyValue.key || keyValue['unknown'], keyValue.value);
    });

    if (propertyAccessorResultStrings.length)
        processKeyValue('_ko_property_writers', "{" + propertyAccessorResultStrings.join(",") + " }");

    return resultStrings.join(",");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.expressionRewriting.writeValueToProperty"></a>[function <span class="apidocSignatureSpan">knockout.expressionRewriting.</span>writeValueToProperty (property, allBindings, key, value, checkIfDifferent)](#apidoc.element.knockout.expressionRewriting.writeValueToProperty)
- description and source-code
```javascript
writeValueToProperty = function (property, allBindings, key, value, checkIfDifferent) {
    if (!property || !ko.isObservable(property)) {
        var propWriters = allBindings.get('_ko_property_writers');
        if (propWriters && propWriters[key])
            propWriters[key](value);
    } else if (ko.isWriteableObservable(property) && (!checkIfDifferent || property.peek() !== value)) {
        property(value);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.expressionRewriting.bindingRewriteValidators"></a>[module knockout.expressionRewriting.bindingRewriteValidators](#apidoc.module.knockout.expressionRewriting.bindingRewriteValidators)

#### <a name="apidoc.element.knockout.expressionRewriting.bindingRewriteValidators.template"></a>[function <span class="apidocSignatureSpan">knockout.expressionRewriting.bindingRewriteValidators.</span>template (bindingValue)](#apidoc.element.knockout.expressionRewriting.bindingRewriteValidators.template)
- description and source-code
```javascript
template = function (bindingValue) {
    var parsedBindingValue = ko.expressionRewriting.parseObjectLiteral(bindingValue);

    if ((parsedBindingValue.length == 1) && parsedBindingValue[0]['unknown'])
        return null; // It looks like a string literal, not an object literal, so treat it as a named template (which is allowed
 for rewriting)

    if (ko.expressionRewriting.keyValueArrayContainsKey(parsedBindingValue, "name"))
        return null; // Named templates can be rewritten, so return "no error"
    return "This template engine does not support anonymous templates nested within its templates";
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.extenders"></a>[module knockout.extenders](#apidoc.module.knockout.extenders)

#### <a name="apidoc.element.knockout.extenders.deferred"></a>[function <span class="apidocSignatureSpan">knockout.extenders.</span>deferred (target, options)](#apidoc.element.knockout.extenders.deferred)
- description and source-code
```javascript
deferred = function (target, options) {
    if (options !== true) {
        throw new Error('The \'deferred\' extender only accepts the value \'true\', because it is not supported to turn deferral
 off once enabled.')
    }

    if (!target._deferUpdates) {
        target._deferUpdates = true;
        target.limit(function (callback) {
            var handle,
                ignoreUpdates = false;
            return function () {
                if (!ignoreUpdates) {
                    ko.tasks.cancel(handle);
                    handle = ko.tasks.schedule(callback);

                    try {
                        ignoreUpdates = true;
                        target['notifySubscribers'](undefined, 'dirty');
                    } finally {
                        ignoreUpdates = false;
                    }
                }
            };
        });
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.extenders.notify"></a>[function <span class="apidocSignatureSpan">knockout.extenders.</span>notify (target, notifyWhen)](#apidoc.element.knockout.extenders.notify)
- description and source-code
```javascript
notify = function (target, notifyWhen) {
    target["equalityComparer"] = notifyWhen == "always" ?
        null :  // null equalityComparer means to always notify
        valuesArePrimitiveAndEqual;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.extenders.rateLimit"></a>[function <span class="apidocSignatureSpan">knockout.extenders.</span>rateLimit (target, options)](#apidoc.element.knockout.extenders.rateLimit)
- description and source-code
```javascript
rateLimit = function (target, options) {
    var timeout, method, limitFunction;

    if (typeof options == 'number') {
        timeout = options;
    } else {
        timeout = options['timeout'];
        method = options['method'];
    }

    // rateLimit supersedes deferred updates
    target._deferUpdates = false;

    limitFunction = method == 'notifyWhenChangesStop' ?  debounce : throttle;
    target.limit(function(callback) {
        return limitFunction(callback, timeout);
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.extenders.throttle"></a>[function <span class="apidocSignatureSpan">knockout.extenders.</span>throttle (target, timeout)](#apidoc.element.knockout.extenders.throttle)
- description and source-code
```javascript
throttle = function (target, timeout) {
    // Throttling means two things:

    // (1) For dependent observables, we throttle *evaluations* so that, no matter how fast its dependencies
    //     notify updates, the target doesn't re-evaluate (and hence doesn't notify) faster than a certain rate
    target['throttleEvaluation'] = timeout;

    // (2) For writable targets (observables, or writable dependent observables), we throttle *writes*
    //     so the target cannot change value synchronously or faster than a certain rate
    var writeTimeoutInstance = null;
    return ko.dependentObservable({
        'read': target,
        'write': function(value) {
            clearTimeout(writeTimeoutInstance);
            writeTimeoutInstance = ko.utils.setTimeout(function() {
                target(value);
            }, timeout);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.extenders.trackArrayChanges"></a>[function <span class="apidocSignatureSpan">knockout.extenders.</span>trackArrayChanges (target, options)](#apidoc.element.knockout.extenders.trackArrayChanges)
- description and source-code
```javascript
trackArrayChanges = function (target, options) {
    // Use the provided options--each call to trackArrayChanges overwrites the previously set options
    target.compareArrayOptions = {};
    if (options && typeof options == "object") {
        ko.utils.extend(target.compareArrayOptions, options);
    }
    target.compareArrayOptions['sparse'] = true;

    // Only modify the target observable once
    if (target.cacheDiffForKnownOperation) {
        return;
    }
    var trackingChanges = false,
        cachedDiff = null,
        arrayChangeSubscription,
        pendingNotifications = 0,
        underlyingNotifySubscribersFunction,
        underlyingBeforeSubscriptionAddFunction = target.beforeSubscriptionAdd,
        underlyingAfterSubscriptionRemoveFunction = target.afterSubscriptionRemove;

    // Watch "subscribe" calls, and for array change events, ensure change tracking is enabled
    target.beforeSubscriptionAdd = function (event) {
        if (underlyingBeforeSubscriptionAddFunction)
            underlyingBeforeSubscriptionAddFunction.call(target, event);
        if (event === arrayChangeEventName) {
            trackChanges();
        }
    };
    // Watch "dispose" calls, and for array change events, ensure change tracking is disabled when all are disposed
    target.afterSubscriptionRemove = function (event) {
        if (underlyingAfterSubscriptionRemoveFunction)
            underlyingAfterSubscriptionRemoveFunction.call(target, event);
        if (event === arrayChangeEventName && !target.hasSubscriptionsForEvent(arrayChangeEventName)) {
            if (underlyingNotifySubscribersFunction) {
                target['notifySubscribers'] = underlyingNotifySubscribersFunction;
                underlyingNotifySubscribersFunction = undefined;
            }
            arrayChangeSubscription.dispose();
            trackingChanges = false;
        }
    };

    function trackChanges() {
        // Calling 'trackChanges' multiple times is the same as calling it once
        if (trackingChanges) {
            return;
        }

        trackingChanges = true;

        // Intercept "notifySubscribers" to track how many times it was called.
        underlyingNotifySubscribersFunction = target['notifySubscribers'];
        target['notifySubscribers'] = function(valueToNotify, event) {
            if (!event || event === defaultEvent) {
                ++pendingNotifications;
            }
            return underlyingNotifySubscribersFunction.apply(this, arguments);
        };

        // Each time the array changes value, capture a clone so that on the next
        // change it's possible to produce a diff
        var previousContents = [].concat(target.peek() || []);
        cachedDiff = null;
        arrayChangeSubscription = target.subscribe(function(currentContents) {
            // Make a copy of the current contents and ensure it's an array
            currentContents = [].concat(currentContents || []);

            // Compute the diff and issue notifications, but only if someone is listening
            if (target.hasSubscriptionsForEvent(arrayChangeEventName)) {
                var changes = getChanges(previousContents, currentContents);
            }

            // Eliminate references to the old, removed items, so they can be GCed
            previousContents = currentContents;
            cachedDiff = null;
            pendingNotifications = 0;

            if (changes && changes.length) {
                target['notifySubscribers'](changes, arrayChangeEventName);
            }
        });
    }

    function getChanges(previousContents, currentContents) {
        // We try to re-use cached diffs.
        // The scenarios where pendingNotifications > 1 are when using rate-limiting or the Deferred Updates
        // plugin, which without this check would not be compatible with arrayChange notifications. Normally,
        // notifications are issued immediately so we wouldn't be queueing up more than one.
        if (!cachedDiff || pendingNotifications > 1) {
            cachedDiff = ko.utils.compareArrays(previousContents, curr ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.jqueryTmplTemplateEngine"></a>[module knockout.jqueryTmplTemplateEngine](#apidoc.module.knockout.jqueryTmplTemplateEngine)

#### <a name="apidoc.element.knockout.jqueryTmplTemplateEngine.jqueryTmplTemplateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>jqueryTmplTemplateEngine ()](#apidoc.element.knockout.jqueryTmplTemplateEngine.jqueryTmplTemplateEngine)
- description and source-code
```javascript
jqueryTmplTemplateEngine = function () {
    // Detect which version of jquery-tmpl you're using. Unfortunately jquery-tmpl
    // doesn't expose a version number, so we have to infer it.
    // Note that as of Knockout 1.3, we only support jQuery.tmpl 1.0.0pre and later,
    // which KO internally refers to as version "2", so older versions are no longer detected.
    var jQueryTmplVersion = this.jQueryTmplVersion = (function() {
        if (!jQueryInstance || !(jQueryInstance['tmpl']))
            return 0;
        // Since it exposes no official version number, we use our own numbering system. To be updated as jquery-tmpl evolves.
        try {
            if (jQueryInstance['tmpl']['tag']['tmpl']['open'].toString().indexOf('__') >= 0) {
                // Since 1.0.0pre, custom tags should append markup to an array called "__"
                return 2; // Final version of jquery.tmpl
            }
        } catch(ex) { /* Apparently not the version we were looking for */ }

        return 1; // Any older version that we don't support
    })();

    function ensureHasReferencedJQueryTemplates() {
        if (jQueryTmplVersion < 2)
            throw new Error("Your version of jQuery.tmpl is too old. Please upgrade to jQuery.tmpl 1.0.0pre or later.");
    }

    function executeTemplate(compiledTemplate, data, jQueryTemplateOptions) {
        return jQueryInstance['tmpl'](compiledTemplate, data, jQueryTemplateOptions);
    }

    this['renderTemplateSource'] = function(templateSource, bindingContext, options, templateDocument) {
        templateDocument = templateDocument || document;
        options = options || {};
        ensureHasReferencedJQueryTemplates();

        // Ensure we have stored a precompiled version of this template (don't want to reparse on every render)
        var precompiled = templateSource['data']('precompiled');
        if (!precompiled) {
            var templateText = templateSource['text']() || "";
            // Wrap in "with($whatever.koBindingContext) { ... }"
            templateText = "{{ko_with $item.koBindingContext}}" + templateText + "{{/ko_with}}";

            precompiled = jQueryInstance['template'](null, templateText);
            templateSource['data']('precompiled', precompiled);
        }

        var data = [bindingContext['$data']]; // Prewrap the data in an array to stop jquery.tmpl from trying to unwrap any arrays
        var jQueryTemplateOptions = jQueryInstance['extend']({ 'koBindingContext': bindingContext }, options['templateOptions']);

        var resultNodes = executeTemplate(precompiled, data, jQueryTemplateOptions);
        resultNodes['appendTo'](templateDocument.createElement("div")); // Using "appendTo" forces jQuery/jQuery.tmpl to perform
 necessary cleanup work

        jQueryInstance['fragments'] = {}; // Clear jQuery's fragment cache to avoid a memory leak after a large number of template
 renders
        return resultNodes;
    };

    this['createJavaScriptEvaluatorBlock'] = function(script) {
        return "{{ko_code ((function() { return " + script + " })()) }}";
    };

    this['addTemplate'] = function(templateName, templateMarkup) {
        document.write("<script type='text/html' id='" + templateName + "'>" + templateMarkup + "<" + "/script>");
    };

    if (jQueryTmplVersion > 0) {
        jQueryInstance['tmpl']['tag']['ko_code'] = {
            open: "__.push($1 || '');"
        };
        jQueryInstance['tmpl']['tag']['ko_with'] = {
            open: "with($1) {",
            close: "} "
        };
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.jqueryTmplTemplateEngine.prototype"></a>[module knockout.jqueryTmplTemplateEngine.prototype](#apidoc.module.knockout.jqueryTmplTemplateEngine.prototype)

#### <a name="apidoc.element.knockout.jqueryTmplTemplateEngine.prototype.constructor"></a>[function <span class="apidocSignatureSpan">knockout.jqueryTmplTemplateEngine.prototype.</span>constructor ()](#apidoc.element.knockout.jqueryTmplTemplateEngine.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    // Detect which version of jquery-tmpl you're using. Unfortunately jquery-tmpl
    // doesn't expose a version number, so we have to infer it.
    // Note that as of Knockout 1.3, we only support jQuery.tmpl 1.0.0pre and later,
    // which KO internally refers to as version "2", so older versions are no longer detected.
    var jQueryTmplVersion = this.jQueryTmplVersion = (function() {
        if (!jQueryInstance || !(jQueryInstance['tmpl']))
            return 0;
        // Since it exposes no official version number, we use our own numbering system. To be updated as jquery-tmpl evolves.
        try {
            if (jQueryInstance['tmpl']['tag']['tmpl']['open'].toString().indexOf('__') >= 0) {
                // Since 1.0.0pre, custom tags should append markup to an array called "__"
                return 2; // Final version of jquery.tmpl
            }
        } catch(ex) { /* Apparently not the version we were looking for */ }

        return 1; // Any older version that we don't support
    })();

    function ensureHasReferencedJQueryTemplates() {
        if (jQueryTmplVersion < 2)
            throw new Error("Your version of jQuery.tmpl is too old. Please upgrade to jQuery.tmpl 1.0.0pre or later.");
    }

    function executeTemplate(compiledTemplate, data, jQueryTemplateOptions) {
        return jQueryInstance['tmpl'](compiledTemplate, data, jQueryTemplateOptions);
    }

    this['renderTemplateSource'] = function(templateSource, bindingContext, options, templateDocument) {
        templateDocument = templateDocument || document;
        options = options || {};
        ensureHasReferencedJQueryTemplates();

        // Ensure we have stored a precompiled version of this template (don't want to reparse on every render)
        var precompiled = templateSource['data']('precompiled');
        if (!precompiled) {
            var templateText = templateSource['text']() || "";
            // Wrap in "with($whatever.koBindingContext) { ... }"
            templateText = "{{ko_with $item.koBindingContext}}" + templateText + "{{/ko_with}}";

            precompiled = jQueryInstance['template'](null, templateText);
            templateSource['data']('precompiled', precompiled);
        }

        var data = [bindingContext['$data']]; // Prewrap the data in an array to stop jquery.tmpl from trying to unwrap any arrays
        var jQueryTemplateOptions = jQueryInstance['extend']({ 'koBindingContext': bindingContext }, options['templateOptions']);

        var resultNodes = executeTemplate(precompiled, data, jQueryTemplateOptions);
        resultNodes['appendTo'](templateDocument.createElement("div")); // Using "appendTo" forces jQuery/jQuery.tmpl to perform
 necessary cleanup work

        jQueryInstance['fragments'] = {}; // Clear jQuery's fragment cache to avoid a memory leak after a large number of template
 renders
        return resultNodes;
    };

    this['createJavaScriptEvaluatorBlock'] = function(script) {
        return "{{ko_code ((function() { return " + script + " })()) }}";
    };

    this['addTemplate'] = function(templateName, templateMarkup) {
        document.write("<script type='text/html' id='" + templateName + "'>" + templateMarkup + "<" + "/script>");
    };

    if (jQueryTmplVersion > 0) {
        jQueryInstance['tmpl']['tag']['ko_code'] = {
            open: "__.push($1 || '');"
        };
        jQueryInstance['tmpl']['tag']['ko_with'] = {
            open: "with($1) {",
            close: "} "
        };
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.memoization"></a>[module knockout.memoization](#apidoc.module.knockout.memoization)

#### <a name="apidoc.element.knockout.memoization.memoize"></a>[function <span class="apidocSignatureSpan">knockout.memoization.</span>memoize (callback)](#apidoc.element.knockout.memoization.memoize)
- description and source-code
```javascript
memoize = function (callback) {
    if (typeof callback != "function")
        throw new Error("You can only pass a function to ko.memoization.memoize()");
    var memoId = generateRandomId();
    memos[memoId] = callback;
    return "<!--[ko_memo:" + memoId + "]-->";
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.memoization.parseMemoText"></a>[function <span class="apidocSignatureSpan">knockout.memoization.</span>parseMemoText (memoText)](#apidoc.element.knockout.memoization.parseMemoText)
- description and source-code
```javascript
parseMemoText = function (memoText) {
    var match = memoText.match(/^\[ko_memo\:(.*?)\]$/);
    return match ? match[1] : null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.memoization.unmemoize"></a>[function <span class="apidocSignatureSpan">knockout.memoization.</span>unmemoize (memoId, callbackParams)](#apidoc.element.knockout.memoization.unmemoize)
- description and source-code
```javascript
unmemoize = function (memoId, callbackParams) {
    var callback = memos[memoId];
    if (callback === undefined)
        throw new Error("Couldn't find any memo with ID " + memoId + ". Perhaps it's already been unmemoized.");
    try {
        callback.apply(null, callbackParams || []);
        return true;
    }
    finally { delete memos[memoId]; }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.memoization.unmemoizeDomNodeAndDescendants"></a>[function <span class="apidocSignatureSpan">knockout.memoization.</span>unmemoizeDomNodeAndDescendants (domNode, extraCallbackParamsArray)](#apidoc.element.knockout.memoization.unmemoizeDomNodeAndDescendants)
- description and source-code
```javascript
unmemoizeDomNodeAndDescendants = function (domNode, extraCallbackParamsArray) {
    var memos = [];
    findMemoNodes(domNode, memos);
    for (var i = 0, j = memos.length; i < j; i++) {
        var node = memos[i].domNode;
        var combinedParams = [node];
        if (extraCallbackParamsArray)
            ko.utils.arrayPushAll(combinedParams, extraCallbackParamsArray);
        ko.memoization.unmemoize(memos[i].memoId, combinedParams);
        node.nodeValue = ""; // Neuter this node so we don't try to unmemoize it again
        if (node.parentNode)
            node.parentNode.removeChild(node); // If possible, erase it totally (not always possible - someone else might just hold
 a reference to it then call unmemoizeDomNodeAndDescendants again)
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.nativeTemplateEngine"></a>[module knockout.nativeTemplateEngine](#apidoc.module.knockout.nativeTemplateEngine)

#### <a name="apidoc.element.knockout.nativeTemplateEngine.nativeTemplateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>nativeTemplateEngine ()](#apidoc.element.knockout.nativeTemplateEngine.nativeTemplateEngine)
- description and source-code
```javascript
nativeTemplateEngine = function () {
    this['allowTemplateRewriting'] = false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.nativeTemplateEngine.prototype"></a>[module knockout.nativeTemplateEngine.prototype](#apidoc.module.knockout.nativeTemplateEngine.prototype)

#### <a name="apidoc.element.knockout.nativeTemplateEngine.prototype.constructor"></a>[function <span class="apidocSignatureSpan">knockout.nativeTemplateEngine.prototype.</span>constructor ()](#apidoc.element.knockout.nativeTemplateEngine.prototype.constructor)
- description and source-code
```javascript
constructor = function () {
    this['allowTemplateRewriting'] = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.nativeTemplateEngine.prototype.renderTemplateSource"></a>[function <span class="apidocSignatureSpan">knockout.nativeTemplateEngine.prototype.</span>renderTemplateSource (templateSource, bindingContext, options, templateDocument)](#apidoc.element.knockout.nativeTemplateEngine.prototype.renderTemplateSource)
- description and source-code
```javascript
renderTemplateSource = function (templateSource, bindingContext, options, templateDocument) {
    var useNodesIfAvailable = !(ko.utils.ieVersion < 9), // IE<9 cloneNode doesn't work properly
        templateNodesFunc = useNodesIfAvailable ? templateSource['nodes'] : null,
        templateNodes = templateNodesFunc ? templateSource['nodes']() : null;

    if (templateNodes) {
        return ko.utils.makeArray(templateNodes.cloneNode(true).childNodes);
    } else {
        var templateText = templateSource['text']();
        return ko.utils.parseHtmlFragment(templateText, templateDocument);
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.selectExtensions"></a>[module knockout.selectExtensions](#apidoc.module.knockout.selectExtensions)

#### <a name="apidoc.element.knockout.selectExtensions.readValue"></a>[function <span class="apidocSignatureSpan">knockout.selectExtensions.</span>readValue (element)](#apidoc.element.knockout.selectExtensions.readValue)
- description and source-code
```javascript
readValue = function (element) {
    switch (ko.utils.tagNameLower(element)) {
        case 'option':
            if (element[hasDomDataExpandoProperty] === true)
                return ko.utils.domData.get(element, ko.bindingHandlers.options.optionValueDomDataKey);
            return ko.utils.ieVersion <= 7
                ? (element.getAttributeNode('value') && element.getAttributeNode('value').specified ? element.value : element.text
)
                : element.value;
        case 'select':
            return element.selectedIndex >= 0 ? ko.selectExtensions.readValue(element.options[element.selectedIndex]) : undefined
;
        default:
            return element.value;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.selectExtensions.writeValue"></a>[function <span class="apidocSignatureSpan">knockout.selectExtensions.</span>writeValue (element, value, allowUnset)](#apidoc.element.knockout.selectExtensions.writeValue)
- description and source-code
```javascript
writeValue = function (element, value, allowUnset) {
    switch (ko.utils.tagNameLower(element)) {
        case 'option':
            switch(typeof value) {
                case "string":
                    ko.utils.domData.set(element, ko.bindingHandlers.options.optionValueDomDataKey, undefined);
                    if (hasDomDataExpandoProperty in element) { // IE <= 8 throws errors if you delete non-existent properties from
 a DOM node
                        delete element[hasDomDataExpandoProperty];
                    }
                    element.value = value;
                    break;
                default:
                    // Store arbitrary object using DomData
                    ko.utils.domData.set(element, ko.bindingHandlers.options.optionValueDomDataKey, value);
                    element[hasDomDataExpandoProperty] = true;

                    // Special treatment of numbers is just for backward compatibility. KO 1.2.1 wrote numerical values to element
.value.
                    element.value = typeof value === "number" ? value : "";
                    break;
            }
            break;
        case 'select':
            if (value === "" || value === null)       // A blank string or null value will select the caption
                value = undefined;
            var selection = -1;
            for (var i = 0, n = element.options.length, optionValue; i < n; ++i) {
                optionValue = ko.selectExtensions.readValue(element.options[i]);
                // Include special check to handle selecting a caption with a blank string value
                if (optionValue == value || (optionValue == "" && value === undefined)) {
                    selection = i;
                    break;
                }
            }
            if (allowUnset || selection >= 0 || (value === undefined && element.size > 1)) {
                element.selectedIndex = selection;
            }
            break;
        default:
            if ((value === null) || (value === undefined))
                value = "";
            element.value = value;
            break;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.subscription"></a>[module knockout.subscription](#apidoc.module.knockout.subscription)

#### <a name="apidoc.element.knockout.subscription.subscription"></a>[function <span class="apidocSignatureSpan">knockout.</span>subscription (target, callback, disposeCallback)](#apidoc.element.knockout.subscription.subscription)
- description and source-code
```javascript
subscription = function (target, callback, disposeCallback) {
    this._target = target;
    this.callback = callback;
    this.disposeCallback = disposeCallback;
    this.isDisposed = false;
    ko.exportProperty(this, 'dispose', this.dispose);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.subscription.prototype"></a>[module knockout.subscription.prototype](#apidoc.module.knockout.subscription.prototype)

#### <a name="apidoc.element.knockout.subscription.prototype.dispose"></a>[function <span class="apidocSignatureSpan">knockout.subscription.prototype.</span>dispose ()](#apidoc.element.knockout.subscription.prototype.dispose)
- description and source-code
```javascript
dispose = function () {
    this.isDisposed = true;
    this.disposeCallback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.tasks"></a>[module knockout.tasks](#apidoc.module.knockout.tasks)

#### <a name="apidoc.element.knockout.tasks.cancel"></a>[function <span class="apidocSignatureSpan">knockout.tasks.</span>cancel (handle)](#apidoc.element.knockout.tasks.cancel)
- description and source-code
```javascript
cancel = function (handle) {
    var index = handle - (nextHandle - taskQueueLength);
    if (index >= nextIndexToProcess && index < taskQueueLength) {
        taskQueue[index] = null;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.tasks.resetForTesting"></a>[function <span class="apidocSignatureSpan">knockout.tasks.</span>resetForTesting ()](#apidoc.element.knockout.tasks.resetForTesting)
- description and source-code
```javascript
resetForTesting = function () {
    var length = taskQueueLength - nextIndexToProcess;
    nextIndexToProcess = taskQueueLength = taskQueue.length = 0;
    return length;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.tasks.runEarly"></a>[function <span class="apidocSignatureSpan">knockout.tasks.</span>runEarly ()](#apidoc.element.knockout.tasks.runEarly)
- description and source-code
```javascript
function processTasks() {
    if (taskQueueLength) {
        // Each mark represents the end of a logical group of tasks and the number of these groups is
        // limited to prevent unchecked recursion.
        var mark = taskQueueLength, countMarks = 0;

        // nextIndexToProcess keeps track of where we are in the queue; processTasks can be called recursively without issue
        for (var task; nextIndexToProcess < taskQueueLength; ) {
            if (task = taskQueue[nextIndexToProcess++]) {
                if (nextIndexToProcess > mark) {
                    if (++countMarks >= 5000) {
                        nextIndexToProcess = taskQueueLength;   // skip all tasks remaining in the queue since any of them could
 be causing the recursion
                        ko.utils.deferError(Error("'Too much recursion' after processing " + countMarks + " task groups."));
                        break;
                    }
                    mark = taskQueueLength;
                }
                try {
                    task();
                } catch (ex) {
                    ko.utils.deferError(ex);
                }
            }
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.tasks.schedule"></a>[function <span class="apidocSignatureSpan">knockout.tasks.</span>schedule (func)](#apidoc.element.knockout.tasks.schedule)
- description and source-code
```javascript
schedule = function (func) {
    if (!taskQueueLength) {
        scheduleTaskProcessing();
    }

    taskQueue[taskQueueLength++] = func;
    return nextHandle++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.tasks.scheduler"></a>[function <span class="apidocSignatureSpan">knockout.tasks.</span>scheduler (callback)](#apidoc.element.knockout.tasks.scheduler)
- description and source-code
```javascript
scheduler = function (callback) {
    setTimeout(callback, 0);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateEngine"></a>[module knockout.templateEngine](#apidoc.module.knockout.templateEngine)

#### <a name="apidoc.element.knockout.templateEngine.templateEngine"></a>[function <span class="apidocSignatureSpan">knockout.</span>templateEngine ()](#apidoc.element.knockout.templateEngine.templateEngine)
- description and source-code
```javascript
templateEngine = function () { }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateEngine.prototype"></a>[module knockout.templateEngine.prototype](#apidoc.module.knockout.templateEngine.prototype)

#### <a name="apidoc.element.knockout.templateEngine.prototype.createJavaScriptEvaluatorBlock"></a>[function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>createJavaScriptEvaluatorBlock (script)](#apidoc.element.knockout.templateEngine.prototype.createJavaScriptEvaluatorBlock)
- description and source-code
```javascript
createJavaScriptEvaluatorBlock = function (script) {
    throw new Error("Override createJavaScriptEvaluatorBlock");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateEngine.prototype.isTemplateRewritten"></a>[function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>isTemplateRewritten (template, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.isTemplateRewritten)
- description and source-code
```javascript
isTemplateRewritten = function (template, templateDocument) {
    // Skip rewriting if requested
    if (this['allowTemplateRewriting'] === false)
        return true;
    return this['makeTemplateSource'](template, templateDocument)['data']("isRewritten");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateEngine.prototype.makeTemplateSource"></a>[function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>makeTemplateSource (template, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.makeTemplateSource)
- description and source-code
```javascript
makeTemplateSource = function (template, templateDocument) {
    // Named template
    if (typeof template == "string") {
        templateDocument = templateDocument || document;
        var elem = templateDocument.getElementById(template);
        if (!elem)
            throw new Error("Cannot find template with ID " + template);
        return new ko.templateSources.domElement(elem);
    } else if ((template.nodeType == 1) || (template.nodeType == 8)) {
        // Anonymous template
        return new ko.templateSources.anonymousTemplate(template);
    } else
        throw new Error("Unknown template type: " + template);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateEngine.prototype.renderTemplate"></a>[function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>renderTemplate (template, bindingContext, options, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.renderTemplate)
- description and source-code
```javascript
renderTemplate = function (template, bindingContext, options, templateDocument) {
    var templateSource = this['makeTemplateSource'](template, templateDocument);
    return this['renderTemplateSource'](templateSource, bindingContext, options, templateDocument);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateEngine.prototype.renderTemplateSource"></a>[function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>renderTemplateSource (templateSource, bindingContext, options, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.renderTemplateSource)
- description and source-code
```javascript
renderTemplateSource = function (templateSource, bindingContext, options, templateDocument) {
    throw new Error("Override renderTemplateSource");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateEngine.prototype.rewriteTemplate"></a>[function <span class="apidocSignatureSpan">knockout.templateEngine.prototype.</span>rewriteTemplate (template, rewriterCallback, templateDocument)](#apidoc.element.knockout.templateEngine.prototype.rewriteTemplate)
- description and source-code
```javascript
rewriteTemplate = function (template, rewriterCallback, templateDocument) {
    var templateSource = this['makeTemplateSource'](template, templateDocument);
    var rewritten = rewriterCallback(templateSource['text']());
    templateSource['text'](rewritten);
    templateSource['data']("isRewritten", true);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateRewriting"></a>[module knockout.templateRewriting](#apidoc.module.knockout.templateRewriting)

#### <a name="apidoc.element.knockout.templateRewriting.applyMemoizedBindingsToNextSibling"></a>[function <span class="apidocSignatureSpan">knockout.templateRewriting.</span>applyMemoizedBindingsToNextSibling (bindings, nodeName)](#apidoc.element.knockout.templateRewriting.applyMemoizedBindingsToNextSibling)
- description and source-code
```javascript
applyMemoizedBindingsToNextSibling = function (bindings, nodeName) {
    return ko.memoization.memoize(function (domNode, bindingContext) {
        var nodeToBind = domNode.nextSibling;
        if (nodeToBind && nodeToBind.nodeName.toLowerCase() === nodeName) {
            ko.applyBindingAccessorsToNode(nodeToBind, bindings, bindingContext);
        }
    });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateRewriting.ensureTemplateIsRewritten"></a>[function <span class="apidocSignatureSpan">knockout.templateRewriting.</span>ensureTemplateIsRewritten (template, templateEngine, templateDocument)](#apidoc.element.knockout.templateRewriting.ensureTemplateIsRewritten)
- description and source-code
```javascript
ensureTemplateIsRewritten = function (template, templateEngine, templateDocument) {
    if (!templateEngine['isTemplateRewritten'](template, templateDocument))
        templateEngine['rewriteTemplate'](template, function (htmlString) {
            return ko.templateRewriting.memoizeBindingAttributeSyntax(htmlString, templateEngine);
        }, templateDocument);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateRewriting.memoizeBindingAttributeSyntax"></a>[function <span class="apidocSignatureSpan">knockout.templateRewriting.</span>memoizeBindingAttributeSyntax (htmlString, templateEngine)](#apidoc.element.knockout.templateRewriting.memoizeBindingAttributeSyntax)
- description and source-code
```javascript
memoizeBindingAttributeSyntax = function (htmlString, templateEngine) {
    return htmlString.replace(memoizeDataBindingAttributeSyntaxRegex, function () {
        return constructMemoizedTagReplacement(/* dataBindAttributeValue: */ arguments[4], /* tagToRetain: */ arguments[1], /* nodeName
: */ arguments[2], templateEngine);
    }).replace(memoizeVirtualContainerBindingSyntaxRegex, function() {
        return constructMemoizedTagReplacement(/* dataBindAttributeValue: */ arguments[1], /* tagToRetain: */ "<!-- ko -->", /*
nodeName: */ "#comment", templateEngine);
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateSources"></a>[module knockout.templateSources](#apidoc.module.knockout.templateSources)

#### <a name="apidoc.element.knockout.templateSources.anonymousTemplate"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.</span>anonymousTemplate (element)](#apidoc.element.knockout.templateSources.anonymousTemplate)
- description and source-code
```javascript
anonymousTemplate = function (element) {
    this.domElement = element;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateSources.domElement"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.</span>domElement (element)](#apidoc.element.knockout.templateSources.domElement)
- description and source-code
```javascript
domElement = function (element) {
    this.domElement = element;

    if (element) {
        var tagNameLower = ko.utils.tagNameLower(element);
        this.templateType =
            tagNameLower === "script" ? templateScript :
            tagNameLower === "textarea" ? templateTextArea :
                // For browsers with proper <template> element support, where the .content property gives a document fragment
            tagNameLower == "template" && element.content && element.content.nodeType === 11 ? templateTemplate :
            templateElement;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateSources.anonymousTemplate"></a>[module knockout.templateSources.anonymousTemplate](#apidoc.module.knockout.templateSources.anonymousTemplate)

#### <a name="apidoc.element.knockout.templateSources.anonymousTemplate.anonymousTemplate"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.</span>anonymousTemplate (element)](#apidoc.element.knockout.templateSources.anonymousTemplate.anonymousTemplate)
- description and source-code
```javascript
anonymousTemplate = function (element) {
    this.domElement = element;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateSources.anonymousTemplate.prototype"></a>[module knockout.templateSources.anonymousTemplate.prototype](#apidoc.module.knockout.templateSources.anonymousTemplate.prototype)

#### <a name="apidoc.element.knockout.templateSources.anonymousTemplate.prototype.constructor"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.anonymousTemplate.prototype.</span>constructor (element)](#apidoc.element.knockout.templateSources.anonymousTemplate.prototype.constructor)
- description and source-code
```javascript
constructor = function (element) {
    this.domElement = element;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateSources.anonymousTemplate.prototype.text"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.anonymousTemplate.prototype.</span>text ()](#apidoc.element.knockout.templateSources.anonymousTemplate.prototype.text)
- description and source-code
```javascript
text = function () {
    if (arguments.length == 0) {
        var templateData = getTemplateDomData(this.domElement);
        if (templateData.textData === undefined && templateData.containerData)
            templateData.textData = templateData.containerData.innerHTML;
        return templateData.textData;
    } else {
        var valueToWrite = arguments[0];
        setTemplateDomData(this.domElement, {textData: valueToWrite});
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateSources.domElement"></a>[module knockout.templateSources.domElement](#apidoc.module.knockout.templateSources.domElement)

#### <a name="apidoc.element.knockout.templateSources.domElement.domElement"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.</span>domElement (element)](#apidoc.element.knockout.templateSources.domElement.domElement)
- description and source-code
```javascript
domElement = function (element) {
    this.domElement = element;

    if (element) {
        var tagNameLower = ko.utils.tagNameLower(element);
        this.templateType =
            tagNameLower === "script" ? templateScript :
            tagNameLower === "textarea" ? templateTextArea :
                // For browsers with proper <template> element support, where the .content property gives a document fragment
            tagNameLower == "template" && element.content && element.content.nodeType === 11 ? templateTemplate :
            templateElement;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.templateSources.domElement.prototype"></a>[module knockout.templateSources.domElement.prototype](#apidoc.module.knockout.templateSources.domElement.prototype)

#### <a name="apidoc.element.knockout.templateSources.domElement.prototype.data"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.domElement.prototype.</span>data (key)](#apidoc.element.knockout.templateSources.domElement.prototype.data)
- description and source-code
```javascript
data = function (key) {
    if (arguments.length === 1) {
        return ko.utils.domData.get(this.domElement, dataDomDataPrefix + key);
    } else {
        ko.utils.domData.set(this.domElement, dataDomDataPrefix + key, arguments[1]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateSources.domElement.prototype.nodes"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.domElement.prototype.</span>nodes ()](#apidoc.element.knockout.templateSources.domElement.prototype.nodes)
- description and source-code
```javascript
nodes = function () {
    var element = this.domElement;
    if (arguments.length == 0) {
        var templateData = getTemplateDomData(element),
            containerData = templateData.containerData;
        return containerData || (
            this.templateType === templateTemplate ? element.content :
            this.templateType === templateElement ? element :
            undefined);
    } else {
        var valueToWrite = arguments[0];
        setTemplateDomData(element, {containerData: valueToWrite});
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.templateSources.domElement.prototype.text"></a>[function <span class="apidocSignatureSpan">knockout.templateSources.domElement.prototype.</span>text ()](#apidoc.element.knockout.templateSources.domElement.prototype.text)
- description and source-code
```javascript
text = function () {
    var elemContentsProperty = this.templateType === templateScript ? "text"
                             : this.templateType === templateTextArea ? "value"
                             : "innerHTML";

    if (arguments.length == 0) {
        return this.domElement[elemContentsProperty];
    } else {
        var valueToWrite = arguments[0];
        if (elemContentsProperty === "innerHTML")
            ko.utils.setHtml(this.domElement, valueToWrite);
        else
            this.domElement[elemContentsProperty] = valueToWrite;
    }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.utils"></a>[module knockout.utils](#apidoc.module.knockout.utils)

#### <a name="apidoc.element.knockout.utils.addOrRemoveItem"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>addOrRemoveItem (array, value, included)](#apidoc.element.knockout.utils.addOrRemoveItem)
- description and source-code
```javascript
addOrRemoveItem = function (array, value, included) {
    var existingEntryIndex = ko.utils.arrayIndexOf(ko.utils.peekObservable(array), value);
    if (existingEntryIndex < 0) {
        if (included)
            array.push(value);
    } else {
        if (!included)
            array.splice(existingEntryIndex, 1);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.anyDomNodeIsAttachedToDocument"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>anyDomNodeIsAttachedToDocument (nodes)](#apidoc.element.knockout.utils.anyDomNodeIsAttachedToDocument)
- description and source-code
```javascript
anyDomNodeIsAttachedToDocument = function (nodes) {
    return !!ko.utils.arrayFirst(nodes, ko.utils.domNodeIsAttachedToDocument);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayFilter"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayFilter (array, predicate)](#apidoc.element.knockout.utils.arrayFilter)
- description and source-code
```javascript
arrayFilter = function (array, predicate) {
    array = array || [];
    var result = [];
    for (var i = 0, j = array.length; i < j; i++)
        if (predicate(array[i], i))
            result.push(array[i]);
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayFirst"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayFirst (array, predicate, predicateOwner)](#apidoc.element.knockout.utils.arrayFirst)
- description and source-code
```javascript
arrayFirst = function (array, predicate, predicateOwner) {
    for (var i = 0, j = array.length; i < j; i++)
        if (predicate.call(predicateOwner, array[i], i))
            return array[i];
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayForEach"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayForEach (array, action)](#apidoc.element.knockout.utils.arrayForEach)
- description and source-code
```javascript
arrayForEach = function (array, action) {
    for (var i = 0, j = array.length; i < j; i++)
        action(array[i], i);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayGetDistinctValues"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayGetDistinctValues (array)](#apidoc.element.knockout.utils.arrayGetDistinctValues)
- description and source-code
```javascript
arrayGetDistinctValues = function (array) {
    array = array || [];
    var result = [];
    for (var i = 0, j = array.length; i < j; i++) {
        if (ko.utils.arrayIndexOf(result, array[i]) < 0)
            result.push(array[i]);
    }
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayIndexOf"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayIndexOf (array, item)](#apidoc.element.knockout.utils.arrayIndexOf)
- description and source-code
```javascript
arrayIndexOf = function (array, item) {
    if (typeof Array.prototype.indexOf == "function")
        return Array.prototype.indexOf.call(array, item);
    for (var i = 0, j = array.length; i < j; i++)
        if (array[i] === item)
            return i;
    return -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayMap"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayMap (array, mapping)](#apidoc.element.knockout.utils.arrayMap)
- description and source-code
```javascript
arrayMap = function (array, mapping) {
    array = array || [];
    var result = [];
    for (var i = 0, j = array.length; i < j; i++)
        result.push(mapping(array[i], i));
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayPushAll"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayPushAll (array, valuesToPush)](#apidoc.element.knockout.utils.arrayPushAll)
- description and source-code
```javascript
arrayPushAll = function (array, valuesToPush) {
    if (valuesToPush instanceof Array)
        array.push.apply(array, valuesToPush);
    else
        for (var i = 0, j = valuesToPush.length; i < j; i++)
            array.push(valuesToPush[i]);
    return array;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.arrayRemoveItem"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>arrayRemoveItem (array, itemToRemove)](#apidoc.element.knockout.utils.arrayRemoveItem)
- description and source-code
```javascript
arrayRemoveItem = function (array, itemToRemove) {
    var index = ko.utils.arrayIndexOf(array, itemToRemove);
    if (index > 0) {
        array.splice(index, 1);
    }
    else if (index === 0) {
        array.shift();
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.catchFunctionErrors"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>catchFunctionErrors (delegate)](#apidoc.element.knockout.utils.catchFunctionErrors)
- description and source-code
```javascript
catchFunctionErrors = function (delegate) {
    return ko['onError'] ? function () {
        try {
            return delegate.apply(this, arguments);
        } catch (e) {
            ko['onError'] && ko['onError'](e);
            throw e;
        }
    } : delegate;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.cloneNodes"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>cloneNodes (nodesArray, shouldCleanNodes)](#apidoc.element.knockout.utils.cloneNodes)
- description and source-code
```javascript
cloneNodes = function (nodesArray, shouldCleanNodes) {
    for (var i = 0, j = nodesArray.length, newNodesArray = []; i < j; i++) {
        var clonedNode = nodesArray[i].cloneNode(true);
        newNodesArray.push(shouldCleanNodes ? ko.cleanNode(clonedNode) : clonedNode);
    }
    return newNodesArray;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.compareArrays"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>compareArrays (oldArray, newArray, options)](#apidoc.element.knockout.utils.compareArrays)
- description and source-code
```javascript
function compareArrays(oldArray, newArray, options) {
    // For backward compatibility, if the third arg is actually a bool, interpret
    // it as the old parameter 'dontLimitMoves'. Newer code should use { dontLimitMoves: true }.
    options = (typeof options === 'boolean') ? { 'dontLimitMoves': options } : (options || {});
    oldArray = oldArray || [];
    newArray = newArray || [];

    if (oldArray.length < newArray.length)
        return compareSmallArrayToBigArray(oldArray, newArray, statusNotInOld, statusNotInNew, options);
    else
        return compareSmallArrayToBigArray(newArray, oldArray, statusNotInNew, statusNotInOld, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.createSymbolOrString"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>createSymbolOrString (identifier)](#apidoc.element.knockout.utils.createSymbolOrString)
- description and source-code
```javascript
createSymbolOrString = function (identifier) {
    return canUseSymbols ? Symbol(identifier) : identifier;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.deferError"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>deferError (error)](#apidoc.element.knockout.utils.deferError)
- description and source-code
```javascript
deferError = function (error) {
    setTimeout(function () {
        ko['onError'] && ko['onError'](error);
        throw error;
    }, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domNodeIsAttachedToDocument"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>domNodeIsAttachedToDocument (node)](#apidoc.element.knockout.utils.domNodeIsAttachedToDocument)
- description and source-code
```javascript
domNodeIsAttachedToDocument = function (node) {
    return ko.utils.domNodeIsContainedBy(node, node.ownerDocument.documentElement);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domNodeIsContainedBy"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>domNodeIsContainedBy (node, containedByNode)](#apidoc.element.knockout.utils.domNodeIsContainedBy)
- description and source-code
```javascript
domNodeIsContainedBy = function (node, containedByNode) {
    if (node === containedByNode)
        return true;
    if (node.nodeType === 11)
        return false; // Fixes issue #1162 - can't use node.contains for document fragments on IE8
    if (containedByNode.contains)
        return containedByNode.contains(node.nodeType === 3 ? node.parentNode : node);
    if (containedByNode.compareDocumentPosition)
        return (containedByNode.compareDocumentPosition(node) & 16) == 16;
    while (node && node != containedByNode) {
        node = node.parentNode;
    }
    return !!node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.emptyDomNode"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>emptyDomNode (domNode)](#apidoc.element.knockout.utils.emptyDomNode)
- description and source-code
```javascript
emptyDomNode = function (domNode) {
    while (domNode.firstChild) {
        ko.removeNode(domNode.firstChild);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.ensureSelectElementIsRenderedCorrectly"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>ensureSelectElementIsRenderedCorrectly (selectElement)](#apidoc.element.knockout.utils.ensureSelectElementIsRenderedCorrectly)
- description and source-code
```javascript
ensureSelectElementIsRenderedCorrectly = function (selectElement) {
    // Workaround for IE9 rendering bug - it doesn't reliably display all the text in dynamically-added select boxes unless you
force it to re-render by updating the width.
    // (See https://github.com/SteveSanderson/knockout/issues/312, http://stackoverflow.com/questions/5908494/select-only-shows-
first-char-of-selected-option)
    // Also fixes IE7 and IE8 bug that causes selects to be zero width if enclosed by 'if' or 'with'. (See issue #839)
    if (ieVersion) {
        var originalWidth = selectElement.style.width;
        selectElement.style.width = 0;
        selectElement.style.width = originalWidth;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.extend"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>extend (target, source)](#apidoc.element.knockout.utils.extend)
- description and source-code
```javascript
function extend(target, source) {
    if (source) {
        for(var prop in source) {
            if(source.hasOwnProperty(prop)) {
                target[prop] = source[prop];
            }
        }
    }
    return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.findMovesInArrayComparison"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>findMovesInArrayComparison (left, right, limitFailedCompares)](#apidoc.element.knockout.utils.findMovesInArrayComparison)
- description and source-code
```javascript
findMovesInArrayComparison = function (left, right, limitFailedCompares) {
    if (left.length && right.length) {
        var failedCompares, l, r, leftItem, rightItem;
        for (failedCompares = l = 0; (!limitFailedCompares || failedCompares < limitFailedCompares) && (leftItem = left[l]); ++l
) {
            for (r = 0; rightItem = right[r]; ++r) {
                if (leftItem['value'] === rightItem['value']) {
                    leftItem['moved'] = rightItem['index'];
                    rightItem['moved'] = leftItem['index'];
                    right.splice(r, 1);         // This item is marked as moved; so remove it from right list
                    failedCompares = r = 0;     // Reset failed compares count because we're checking for consecutive failures
                    break;
                }
            }
            failedCompares += r;
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.fixUpContinuousNodeArray"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>fixUpContinuousNodeArray (continuousNodeArray, parentNode)](#apidoc.element.knockout.utils.fixUpContinuousNodeArray)
- description and source-code
```javascript
fixUpContinuousNodeArray = function (continuousNodeArray, parentNode) {
    // Before acting on a set of nodes that were previously outputted by a template function, we have to reconcile
    // them against what is in the DOM right now. It may be that some of the nodes have already been removed, or that
    // new nodes might have been inserted in the middle, for example by a binding. Also, there may previously have been
    // leading comment nodes (created by rewritten string-based templates) that have since been removed during binding.
    // So, this function translates the old "map" output array into its best guess of the set of current DOM nodes.
    //
    // Rules:
    //   [A] Any leading nodes that have been removed should be ignored
    //       These most likely correspond to memoization nodes that were already removed during binding
    //       See https://github.com/knockout/knockout/pull/440
    //   [B] Any trailing nodes that have been remove should be ignored
    //       This prevents the code here from adding unrelated nodes to the array while processing rule [C]
    //       See https://github.com/knockout/knockout/pull/1903
    //   [C] We want to output a continuous series of nodes. So, ignore any nodes that have already been removed,
    //       and include any nodes that have been inserted among the previous collection

    if (continuousNodeArray.length) {
        // The parent node can be a virtual element; so get the real parent node
        parentNode = (parentNode.nodeType === 8 && parentNode.parentNode) || parentNode;

        // Rule [A]
        while (continuousNodeArray.length && continuousNodeArray[0].parentNode !== parentNode)
            continuousNodeArray.splice(0, 1);

        // Rule [B]
        while (continuousNodeArray.length > 1 && continuousNodeArray[continuousNodeArray.length - 1].parentNode !== parentNode)
            continuousNodeArray.length--;

        // Rule [C]
        if (continuousNodeArray.length > 1) {
            var current = continuousNodeArray[0], last = continuousNodeArray[continuousNodeArray.length - 1];
            // Replace with the actual new continuous node set
            continuousNodeArray.length = 0;
            while (current !== last) {
                continuousNodeArray.push(current);
                current = current.nextSibling;
            }
            continuousNodeArray.push(last);
        }
    }
    return continuousNodeArray;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.forceRefresh"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>forceRefresh (node)](#apidoc.element.knockout.utils.forceRefresh)
- description and source-code
```javascript
forceRefresh = function (node) {
    // Workaround for an IE9 rendering bug - https://github.com/SteveSanderson/knockout/issues/209
    if (ieVersion >= 9) {
        // For text nodes and comment nodes (most likely virtual elements), we will have to refresh the container
        var elem = node.nodeType == 1 ? node : node.parentNode;
        if (elem.style)
            elem.style.zoom = elem.style.zoom;
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.getFormFields"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>getFormFields (form, fieldName)](#apidoc.element.knockout.utils.getFormFields)
- description and source-code
```javascript
getFormFields = function (form, fieldName) {
    var fields = ko.utils.makeArray(form.getElementsByTagName("input")).concat(ko.utils.makeArray(form.getElementsByTagName("textarea
")));
    var isMatchingField = (typeof fieldName == 'string')
        ? function(field) { return field.name === fieldName }
        : function(field) { return fieldName.test(field.name) }; // Treat fieldName as regex or object containing predicate
    var matches = [];
    for (var i = fields.length - 1; i >= 0; i--) {
        if (isMatchingField(fields[i]))
            matches.push(fields[i]);
    };
    return matches;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.makeArray"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>makeArray (arrayLikeObject)](#apidoc.element.knockout.utils.makeArray)
- description and source-code
```javascript
makeArray = function (arrayLikeObject) {
    var result = [];
    for (var i = 0, j = arrayLikeObject.length; i < j; i++) {
        result.push(arrayLikeObject[i]);
    };
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.moveCleanedNodesToContainerElement"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>moveCleanedNodesToContainerElement (nodes)](#apidoc.element.knockout.utils.moveCleanedNodesToContainerElement)
- description and source-code
```javascript
moveCleanedNodesToContainerElement = function (nodes) {
    // Ensure it's a real array, as we're about to reparent the nodes and
    // we don't want the underlying collection to change while we're doing that.
    var nodesArray = ko.utils.makeArray(nodes);
    var templateDocument = (nodesArray[0] && nodesArray[0].ownerDocument) || document;

    var container = templateDocument.createElement('div');
    for (var i = 0, j = nodesArray.length; i < j; i++) {
        container.appendChild(ko.cleanNode(nodesArray[i]));
    }
    return container;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.objectForEach"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>objectForEach (obj, action)](#apidoc.element.knockout.utils.objectForEach)
- description and source-code
```javascript
function objectForEach(obj, action) {
    for (var prop in obj) {
        if (obj.hasOwnProperty(prop)) {
            action(prop, obj[prop]);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.objectMap"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>objectMap (source, mapping)](#apidoc.element.knockout.utils.objectMap)
- description and source-code
```javascript
objectMap = function (source, mapping) {
    if (!source)
        return source;
    var target = {};
    for (var prop in source) {
        if (source.hasOwnProperty(prop)) {
            target[prop] = mapping(source[prop], prop, source);
        }
    }
    return target;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.parseHtmlFragment"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>parseHtmlFragment (html, documentContext)](#apidoc.element.knockout.utils.parseHtmlFragment)
- description and source-code
```javascript
parseHtmlFragment = function (html, documentContext) {
    return jQueryInstance ?
        jQueryHtmlParse(html, documentContext) :   // As below, benefit from jQuery's optimisations where possible
        simpleHtmlParse(html, documentContext);  // ... otherwise, this simple logic will do in most common cases.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.parseJson"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>parseJson (jsonString)](#apidoc.element.knockout.utils.parseJson)
- description and source-code
```javascript
parseJson = function (jsonString) {
    if (typeof jsonString == "string") {
        jsonString = ko.utils.stringTrim(jsonString);
        if (jsonString) {
            if (JSON && JSON.parse) // Use native parsing where available
                return JSON.parse(jsonString);
            return (new Function("return " + jsonString))(); // Fallback on less safe parsing for older browsers
        }
    }
    return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.peekObservable"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>peekObservable (value)](#apidoc.element.knockout.utils.peekObservable)
- description and source-code
```javascript
peekObservable = function (value) {
    return ko.isObservable(value) ? value.peek() : value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.postJson"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>postJson (urlOrForm, data, options)](#apidoc.element.knockout.utils.postJson)
- description and source-code
```javascript
postJson = function (urlOrForm, data, options) {
    options = options || {};
    var params = options['params'] || {};
    var includeFields = options['includeFields'] || this.fieldsIncludedWithJsonPost;
    var url = urlOrForm;

    // If we were given a form, use its 'action' URL and pick out any requested field values
    if((typeof urlOrForm == 'object') && (ko.utils.tagNameLower(urlOrForm) === "form")) {
        var originalForm = urlOrForm;
        url = originalForm.action;
        for (var i = includeFields.length - 1; i >= 0; i--) {
            var fields = ko.utils.getFormFields(originalForm, includeFields[i]);
            for (var j = fields.length - 1; j >= 0; j--)
                params[fields[j].name] = fields[j].value;
        }
    }

    data = ko.utils.unwrapObservable(data);
    var form = document.createElement("form");
    form.style.display = "none";
    form.action = url;
    form.method = "post";
    for (var key in data) {
        // Since 'data' this is a model object, we include all properties including those inherited from its prototype
        var input = document.createElement("input");
        input.type = "hidden";
        input.name = key;
        input.value = ko.utils.stringifyJson(ko.utils.unwrapObservable(data[key]));
        form.appendChild(input);
    }
    objectForEach(params, function(key, value) {
        var input = document.createElement("input");
        input.type = "hidden";
        input.name = key;
        input.value = value;
        form.appendChild(input);
    });
    document.body.appendChild(form);
    options['submitter'] ? options['submitter'](form) : form.submit();
    setTimeout(function () { form.parentNode.removeChild(form); }, 0);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.range"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>range (min, max)](#apidoc.element.knockout.utils.range)
- description and source-code
```javascript
range = function (min, max) {
    min = ko.utils.unwrapObservable(min);
    max = ko.utils.unwrapObservable(max);
    var result = [];
    for (var i = min; i <= max; i++)
        result.push(i);
    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.registerEventHandler"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>registerEventHandler (element, eventType, handler)](#apidoc.element.knockout.utils.registerEventHandler)
- description and source-code
```javascript
registerEventHandler = function (element, eventType, handler) {
    var wrappedHandler = ko.utils.catchFunctionErrors(handler);

    var mustUseAttachEvent = ieVersion && eventsThatMustBeRegisteredUsingAttachEvent[eventType];
    if (!ko.options['useOnlyNativeEvents'] && !mustUseAttachEvent && jQueryInstance) {
        jQueryInstance(element)['bind'](eventType, wrappedHandler);
    } else if (!mustUseAttachEvent && typeof element.addEventListener == "function")
        element.addEventListener(eventType, wrappedHandler, false);
    else if (typeof element.attachEvent != "undefined") {
        var attachEventHandler = function (event) { wrappedHandler.call(element, event); },
            attachEventName = "on" + eventType;
        element.attachEvent(attachEventName, attachEventHandler);

        // IE does not dispose attachEvent handlers automatically (unlike with addEventListener)
        // so to avoid leaks, we have to remove them manually. See bug #856
        ko.utils.domNodeDisposal.addDisposeCallback(element, function() {
            element.detachEvent(attachEventName, attachEventHandler);
        });
    } else
        throw new Error("Browser doesn't support addEventListener or attachEvent");
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.replaceDomNodes"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>replaceDomNodes (nodeToReplaceOrNodeArray, newNodesArray)](#apidoc.element.knockout.utils.replaceDomNodes)
- description and source-code
```javascript
replaceDomNodes = function (nodeToReplaceOrNodeArray, newNodesArray) {
    var nodesToReplaceArray = nodeToReplaceOrNodeArray.nodeType ? [nodeToReplaceOrNodeArray] : nodeToReplaceOrNodeArray;
    if (nodesToReplaceArray.length > 0) {
        var insertionPoint = nodesToReplaceArray[0];
        var parent = insertionPoint.parentNode;
        for (var i = 0, j = newNodesArray.length; i < j; i++)
            parent.insertBefore(newNodesArray[i], insertionPoint);
        for (var i = 0, j = nodesToReplaceArray.length; i < j; i++) {
            ko.removeNode(nodesToReplaceArray[i]);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setDomNodeChildren"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setDomNodeChildren (domNode, childNodes)](#apidoc.element.knockout.utils.setDomNodeChildren)
- description and source-code
```javascript
setDomNodeChildren = function (domNode, childNodes) {
    ko.utils.emptyDomNode(domNode);
    if (childNodes) {
        for (var i = 0, j = childNodes.length; i < j; i++)
            domNode.appendChild(childNodes[i]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setDomNodeChildrenFromArrayMapping"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setDomNodeChildrenFromArrayMapping (domNode, array, mapping, options, callbackAfterAddingNodes)](#apidoc.element.knockout.utils.setDomNodeChildrenFromArrayMapping)
- description and source-code
```javascript
setDomNodeChildrenFromArrayMapping = function (domNode, array, mapping, options, callbackAfterAddingNodes) {
    // Compare the provided array against the previous one
    array = array || [];
    options = options || {};
    var isFirstExecution = ko.utils.domData.get(domNode, lastMappingResultDomDataKey) === undefined;
    var lastMappingResult = ko.utils.domData.get(domNode, lastMappingResultDomDataKey) || [];
    var lastArray = ko.utils.arrayMap(lastMappingResult, function (x) { return x.arrayEntry; });
    var editScript = ko.utils.compareArrays(lastArray, array, options['dontLimitMoves']);

    // Build the new mapping result
    var newMappingResult = [];
    var lastMappingResultIndex = 0;
    var newMappingResultIndex = 0;

    var nodesToDelete = [];
    var itemsToProcess = [];
    var itemsForBeforeRemoveCallbacks = [];
    var itemsForMoveCallbacks = [];
    var itemsForAfterAddCallbacks = [];
    var mapData;

    function itemMovedOrRetained(editScriptIndex, oldPosition) {
        mapData = lastMappingResult[oldPosition];
        if (newMappingResultIndex !== oldPosition)
            itemsForMoveCallbacks[editScriptIndex] = mapData;
        // Since updating the index might change the nodes, do so before calling fixUpContinuousNodeArray
        mapData.indexObservable(newMappingResultIndex++);
        ko.utils.fixUpContinuousNodeArray(mapData.mappedNodes, domNode);
        newMappingResult.push(mapData);
        itemsToProcess.push(mapData);
    }

    function callCallback(callback, items) {
        if (callback) {
            for (var i = 0, n = items.length; i < n; i++) {
                if (items[i]) {
                    ko.utils.arrayForEach(items[i].mappedNodes, function(node) {
                        callback(node, i, items[i].arrayEntry);
                    });
                }
            }
        }
    }

    for (var i = 0, editScriptItem, movedIndex; editScriptItem = editScript[i]; i++) {
        movedIndex = editScriptItem['moved'];
        switch (editScriptItem['status']) {
            case "deleted":
                if (movedIndex === undefined) {
                    mapData = lastMappingResult[lastMappingResultIndex];

                    // Stop tracking changes to the mapping for these nodes
                    if (mapData.dependentObservable) {
                        mapData.dependentObservable.dispose();
                        mapData.dependentObservable = undefined;
                    }

                    // Queue these nodes for later removal
                    if (ko.utils.fixUpContinuousNodeArray(mapData.mappedNodes, domNode).length) {
                        if (options['beforeRemove']) {
                            newMappingResult.push(mapData);
                            itemsToProcess.push(mapData);
                            if (mapData.arrayEntry === deletedItemDummyValue) {
                                mapData = null;
                            } else {
                                itemsForBeforeRemoveCallbacks[i] = mapData;
                            }
                        }
                        if (mapData) {
                            nodesToDelete.push.apply(nodesToDelete, mapData.mappedNodes);
                        }
                    }
                }
                lastMappingResultIndex++;
                break;

            case "retained":
                itemMovedOrRetained(i, lastMappingResultIndex++);
                break;

            case "added":
                if (movedIndex !== undefined) {
                    itemMovedOrRetained(i, movedIndex);
                } else {
                    mapData = { arrayEntry: editScriptItem['value'], indexObservable: ko.observable(newMappingResultIndex++) };
                    newMappingResult.push(mapData);
                    itemsToProcess.push(mapData);
                    if (!isFirstExecution)
                        itemsForAfterAddCallbacks[i] = mapData;
                }
                break;
        }
    }

    // Store a copy of the array items we just considered so we can difference it next time
    ko. ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setElementName"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setElementName (element, name)](#apidoc.element.knockout.utils.setElementName)
- description and source-code
```javascript
setElementName = function (element, name) {
    element.name = name;

    // Workaround IE 6/7 issue
    // - https://github.com/SteveSanderson/knockout/issues/197
    // - http://www.matts411.com/post/setting_the_name_attribute_in_ie_dom/
    if (ieVersion <= 7) {
        try {
            element.mergeAttributes(document.createElement("<input name='" + element.name + "'/>"), false);
        }
        catch(e) {} // For IE9 with doc mode "IE9 Standards" and browser mode "IE9 Compatibility View"
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setHtml"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setHtml (node, html)](#apidoc.element.knockout.utils.setHtml)
- description and source-code
```javascript
setHtml = function (node, html) {
    ko.utils.emptyDomNode(node);

    // There's no legitimate reason to display a stringified observable without unwrapping it, so we'll unwrap it
    html = ko.utils.unwrapObservable(html);

    if ((html !== null) && (html !== undefined)) {
        if (typeof html != 'string')
            html = html.toString();

        // jQuery contains a lot of sophisticated code to parse arbitrary HTML fragments,
        // for example <tr> elements which are not normally allowed to exist on their own.
        // If you've referenced jQuery we'll use that rather than duplicating its code.
        if (jQueryInstance) {
            jQueryInstance(node)['html'](html);
        } else {
            // ... otherwise, use KO's own parsing logic.
            var parsedNodes = ko.utils.parseHtmlFragment(html, node.ownerDocument);
            for (var i = 0; i < parsedNodes.length; i++)
                node.appendChild(parsedNodes[i]);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setOptionNodeSelectionState"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setOptionNodeSelectionState (optionNode, isSelected)](#apidoc.element.knockout.utils.setOptionNodeSelectionState)
- description and source-code
```javascript
setOptionNodeSelectionState = function (optionNode, isSelected) {
    // IE6 sometimes throws "unknown error" if you try to write to .selected directly, whereas Firefox struggles with setAttribute
. Pick one based on browser.
    if (ieVersion < 7)
        optionNode.setAttribute("selected", isSelected);
    else
        optionNode.selected = isSelected;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setPrototypeOf"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setPrototypeOf (obj, proto)](#apidoc.element.knockout.utils.setPrototypeOf)
- description and source-code
```javascript
function setPrototypeOf(obj, proto) {
    obj.__proto__ = proto;
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setPrototypeOfOrExtend"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setPrototypeOfOrExtend (obj, proto)](#apidoc.element.knockout.utils.setPrototypeOfOrExtend)
- description and source-code
```javascript
function setPrototypeOf(obj, proto) {
    obj.__proto__ = proto;
    return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setTextContent"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setTextContent (element, textContent)](#apidoc.element.knockout.utils.setTextContent)
- description and source-code
```javascript
setTextContent = function (element, textContent) {
    var value = ko.utils.unwrapObservable(textContent);
    if ((value === null) || (value === undefined))
        value = "";

    // We need there to be exactly one child: a text node.
    // If there are no children, more than one, or if it's not a text node,
    // we'll clear everything and create a single text node.
    var innerTextNode = ko.virtualElements.firstChild(element);
    if (!innerTextNode || innerTextNode.nodeType != 3 || ko.virtualElements.nextSibling(innerTextNode)) {
        ko.virtualElements.setDomNodeChildren(element, [element.ownerDocument.createTextNode(value)]);
    } else {
        innerTextNode.data = value;
    }

    ko.utils.forceRefresh(element);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.setTimeout"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>setTimeout (handler, timeout)](#apidoc.element.knockout.utils.setTimeout)
- description and source-code
```javascript
setTimeout = function (handler, timeout) {
    return setTimeout(ko.utils.catchFunctionErrors(handler), timeout);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.stringStartsWith"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>stringStartsWith (string, startsWith)](#apidoc.element.knockout.utils.stringStartsWith)
- description and source-code
```javascript
stringStartsWith = function (string, startsWith) {
    string = string || "";
    if (startsWith.length > string.length)
        return false;
    return string.substring(0, startsWith.length) === startsWith;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.stringTrim"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>stringTrim (string)](#apidoc.element.knockout.utils.stringTrim)
- description and source-code
```javascript
stringTrim = function (string) {
    return string === null || string === undefined ? '' :
        string.trim ?
            string.trim() :
            string.toString().replace(/^[\s\xa0]+|[\s\xa0]+$/g, '');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.stringifyJson"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>stringifyJson (data, replacer, space)](#apidoc.element.knockout.utils.stringifyJson)
- description and source-code
```javascript
stringifyJson = function (data, replacer, space) {   // replacer and space are optional
    if (!JSON || !JSON.stringify)
        throw new Error("Cannot find JSON.stringify(). Some browsers (e.g., IE < 8) don't support it natively, but you can overcome
 this by adding a script reference to json2.js, downloadable from http://www.json.org/json2.js");
    return JSON.stringify(ko.utils.unwrapObservable(data), replacer, space);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.tagNameLower"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>tagNameLower (element)](#apidoc.element.knockout.utils.tagNameLower)
- description and source-code
```javascript
tagNameLower = function (element) {
    // For HTML elements, tagName will always be upper case; for XHTML elements, it'll be lower case.
    // Possible future optimization: If we know it's an element from an XHTML document (not HTML),
    // we don't need to do the .toLowerCase() as it will always be lower case anyway.
    return element && element.tagName && element.tagName.toLowerCase();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.toggleDomNodeCssClass"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>toggleDomNodeCssClass (node, classNames, shouldHaveClass)](#apidoc.element.knockout.utils.toggleDomNodeCssClass)
- description and source-code
```javascript
function toggleDomNodeCssClass(node, classNames, shouldHaveClass) {
    var addOrRemoveFn;
    if (classNames) {
        if (typeof node.classList === 'object') {
            addOrRemoveFn = node.classList[shouldHaveClass ? 'add' : 'remove'];
            ko.utils.arrayForEach(classNames.match(cssClassNameRegex), function(className) {
                addOrRemoveFn.call(node.classList, className);
            });
        } else if (typeof node.className['baseVal'] === 'string') {
            // SVG tag .classNames is an SVGAnimatedString instance
            toggleObjectClassPropertyString(node.className, 'baseVal', classNames, shouldHaveClass);
        } else {
            // node.className ought to be a string.
            toggleObjectClassPropertyString(node, 'className', classNames, shouldHaveClass);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.triggerEvent"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>triggerEvent (element, eventType)](#apidoc.element.knockout.utils.triggerEvent)
- description and source-code
```javascript
triggerEvent = function (element, eventType) {
    if (!(element && element.nodeType))
        throw new Error("element must be a DOM node when calling triggerEvent");

    // For click events on checkboxes and radio buttons, jQuery toggles the element checked state *after* the
    // event handler runs instead of *before*. (This was fixed in 1.9 for checkboxes but not for radio buttons.)
    // IE doesn't change the checked state when you trigger the click event using "fireEvent".
    // In both cases, we'll use the click method instead.
    var useClickWorkaround = isClickOnCheckableElement(element, eventType);

    if (!ko.options['useOnlyNativeEvents'] && jQueryInstance && !useClickWorkaround) {
        jQueryInstance(element)['trigger'](eventType);
    } else if (typeof document.createEvent == "function") {
        if (typeof element.dispatchEvent == "function") {
            var eventCategory = knownEventTypesByEventName[eventType] || "HTMLEvents";
            var event = document.createEvent(eventCategory);
            event.initEvent(eventType, true, true, window, 0, 0, 0, 0, 0, false, false, false, false, 0, element);
            element.dispatchEvent(event);
        }
        else
            throw new Error("The supplied element doesn't support dispatchEvent");
    } else if (useClickWorkaround && element.click) {
        element.click();
    } else if (typeof element.fireEvent != "undefined") {
        element.fireEvent("on" + eventType);
    } else {
        throw new Error("Browser doesn't support triggering events");
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.unwrapObservable"></a>[function <span class="apidocSignatureSpan">knockout.utils.</span>unwrapObservable (value)](#apidoc.element.knockout.utils.unwrapObservable)
- description and source-code
```javascript
unwrapObservable = function (value) {
    return ko.isObservable(value) ? value() : value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.utils.domData"></a>[module knockout.utils.domData](#apidoc.module.knockout.utils.domData)

#### <a name="apidoc.element.knockout.utils.domData.clear"></a>[function <span class="apidocSignatureSpan">knockout.utils.domData.</span>clear (node)](#apidoc.element.knockout.utils.domData.clear)
- description and source-code
```javascript
clear = function (node) {
    var dataStoreKey = node[dataStoreKeyExpandoPropertyName];
    if (dataStoreKey) {
        delete dataStore[dataStoreKey];
        node[dataStoreKeyExpandoPropertyName] = null;
        return true; // Exposing "did clean" flag purely so specs can infer whether things have been cleaned up as intended
    }
    return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domData.get"></a>[function <span class="apidocSignatureSpan">knockout.utils.domData.</span>get (node, key)](#apidoc.element.knockout.utils.domData.get)
- description and source-code
```javascript
get = function (node, key) {
    var allDataForNode = getAll(node, false);
    return allDataForNode === undefined ? undefined : allDataForNode[key];
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domData.nextKey"></a>[function <span class="apidocSignatureSpan">knockout.utils.domData.</span>nextKey ()](#apidoc.element.knockout.utils.domData.nextKey)
- description and source-code
```javascript
nextKey = function () {
    return (uniqueId++) + dataStoreKeyExpandoPropertyName;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domData.set"></a>[function <span class="apidocSignatureSpan">knockout.utils.domData.</span>set (node, key, value)](#apidoc.element.knockout.utils.domData.set)
- description and source-code
```javascript
set = function (node, key, value) {
    if (value === undefined) {
        // Make sure we don't actually create a new domData key if we are actually deleting a value
        if (getAll(node, false) === undefined)
            return;
    }
    var allDataForNode = getAll(node, true);
    allDataForNode[key] = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.utils.domNodeDisposal"></a>[module knockout.utils.domNodeDisposal](#apidoc.module.knockout.utils.domNodeDisposal)

#### <a name="apidoc.element.knockout.utils.domNodeDisposal.addDisposeCallback"></a>[function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>addDisposeCallback (node, callback)](#apidoc.element.knockout.utils.domNodeDisposal.addDisposeCallback)
- description and source-code
```javascript
addDisposeCallback = function (node, callback) {
    if (typeof callback != "function")
        throw new Error("Callback must be a function");
    getDisposeCallbacksCollection(node, true).push(callback);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domNodeDisposal.cleanExternalData"></a>[function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>cleanExternalData (node)](#apidoc.element.knockout.utils.domNodeDisposal.cleanExternalData)
- description and source-code
```javascript
cleanExternalData = function (node) {
    // Special support for jQuery here because it's so commonly used.
    // Many jQuery plugins (including jquery.tmpl) store data using jQuery's equivalent of domData
    // so notify it to tear down any resources associated with the node & descendants here.
    if (jQueryInstance && (typeof jQueryInstance['cleanData'] == "function"))
        jQueryInstance['cleanData']([node]);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domNodeDisposal.cleanNode"></a>[function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>cleanNode (node)](#apidoc.element.knockout.utils.domNodeDisposal.cleanNode)
- description and source-code
```javascript
cleanNode = function (node) {
    // First clean this node, where applicable
    if (cleanableNodeTypes[node.nodeType]) {
        cleanSingleNode(node);

        // ... then its descendants, where applicable
        if (cleanableNodeTypesWithDescendants[node.nodeType]) {
            // Clone the descendants list in case it changes during iteration
            var descendants = [];
            ko.utils.arrayPushAll(descendants, node.getElementsByTagName("*"));
            for (var i = 0, j = descendants.length; i < j; i++)
                cleanSingleNode(descendants[i]);
        }
    }
    return node;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domNodeDisposal.removeDisposeCallback"></a>[function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>removeDisposeCallback (node, callback)](#apidoc.element.knockout.utils.domNodeDisposal.removeDisposeCallback)
- description and source-code
```javascript
removeDisposeCallback = function (node, callback) {
    var callbacksCollection = getDisposeCallbacksCollection(node, false);
    if (callbacksCollection) {
        ko.utils.arrayRemoveItem(callbacksCollection, callback);
        if (callbacksCollection.length == 0)
            destroyCallbacksCollection(node);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.utils.domNodeDisposal.removeNode"></a>[function <span class="apidocSignatureSpan">knockout.utils.domNodeDisposal.</span>removeNode (node)](#apidoc.element.knockout.utils.domNodeDisposal.removeNode)
- description and source-code
```javascript
removeNode = function (node) {
    ko.cleanNode(node);
    if (node.parentNode)
        node.parentNode.removeChild(node);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.knockout.virtualElements"></a>[module knockout.virtualElements](#apidoc.module.knockout.virtualElements)

#### <a name="apidoc.element.knockout.virtualElements.childNodes"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>childNodes (node)](#apidoc.element.knockout.virtualElements.childNodes)
- description and source-code
```javascript
childNodes = function (node) {
    return isStartComment(node) ? getVirtualChildren(node) : node.childNodes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.emptyNode"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>emptyNode (node)](#apidoc.element.knockout.virtualElements.emptyNode)
- description and source-code
```javascript
emptyNode = function (node) {
    if (!isStartComment(node))
        ko.utils.emptyDomNode(node);
    else {
        var virtualChildren = ko.virtualElements.childNodes(node);
        for (var i = 0, j = virtualChildren.length; i < j; i++)
            ko.removeNode(virtualChildren[i]);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.firstChild"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>firstChild (node)](#apidoc.element.knockout.virtualElements.firstChild)
- description and source-code
```javascript
firstChild = function (node) {
    if (!isStartComment(node))
        return node.firstChild;
    if (!node.nextSibling || isEndComment(node.nextSibling))
        return null;
    return node.nextSibling;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.hasBindingValue"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>hasBindingValue (node)](#apidoc.element.knockout.virtualElements.hasBindingValue)
- description and source-code
```javascript
function isStartComment(node) {
    return (node.nodeType == 8) && startCommentRegex.test(commentNodesHaveTextProperty ? node.text : node.nodeValue);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.insertAfter"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>insertAfter (containerNode, nodeToInsert, insertAfterNode)](#apidoc.element.knockout.virtualElements.insertAfter)
- description and source-code
```javascript
insertAfter = function (containerNode, nodeToInsert, insertAfterNode) {
    if (!insertAfterNode) {
        ko.virtualElements.prepend(containerNode, nodeToInsert);
    } else if (!isStartComment(containerNode)) {
        // Insert after insertion point
        if (insertAfterNode.nextSibling)
            containerNode.insertBefore(nodeToInsert, insertAfterNode.nextSibling);
        else
            containerNode.appendChild(nodeToInsert);
    } else {
        // Children of start comments must always have a parent and at least one following sibling (the end comment)
        containerNode.parentNode.insertBefore(nodeToInsert, insertAfterNode.nextSibling);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.nextSibling"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>nextSibling (node)](#apidoc.element.knockout.virtualElements.nextSibling)
- description and source-code
```javascript
nextSibling = function (node) {
    if (isStartComment(node))
        node = getMatchingEndComment(node);
    if (node.nextSibling && isEndComment(node.nextSibling))
        return null;
    return node.nextSibling;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.normaliseVirtualElementDomStructure"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>normaliseVirtualElementDomStructure (elementVerified)](#apidoc.element.knockout.virtualElements.normaliseVirtualElementDomStructure)
- description and source-code
```javascript
normaliseVirtualElementDomStructure = function (elementVerified) {
    // Workaround for https://github.com/SteveSanderson/knockout/issues/155
    // (IE <= 8 or IE 9 quirks mode parses your HTML weirdly, treating closing </li> tags as if they don't exist, thereby moving
 comment nodes
    // that are direct descendants of <ul> into the preceding <li>)
    if (!htmlTagsWithOptionallyClosingChildren[ko.utils.tagNameLower(elementVerified)])
        return;

    // Scan immediate children to see if they contain unbalanced comment tags. If they do, those comment tags
    // must be intended to appear *after* that child, so move them there.
    var childNode = elementVerified.firstChild;
    if (childNode) {
        do {
            if (childNode.nodeType === 1) {
                var unbalancedTags = getUnbalancedChildTags(childNode);
                if (unbalancedTags) {
                    // Fix up the DOM by moving the unbalanced tags to where they most likely were intended to be placed - *after
* the child
                    var nodeToInsertBefore = childNode.nextSibling;
                    for (var i = 0; i < unbalancedTags.length; i++) {
                        if (nodeToInsertBefore)
                            elementVerified.insertBefore(unbalancedTags[i], nodeToInsertBefore);
                        else
                            elementVerified.appendChild(unbalancedTags[i]);
                    }
                }
            }
        } while (childNode = childNode.nextSibling);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.prepend"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>prepend (containerNode, nodeToPrepend)](#apidoc.element.knockout.virtualElements.prepend)
- description and source-code
```javascript
prepend = function (containerNode, nodeToPrepend) {
    if (!isStartComment(containerNode)) {
        if (containerNode.firstChild)
            containerNode.insertBefore(nodeToPrepend, containerNode.firstChild);
        else
            containerNode.appendChild(nodeToPrepend);
    } else {
        // Start comments must always have a parent and at least one following sibling (the end comment)
        containerNode.parentNode.insertBefore(nodeToPrepend, containerNode.nextSibling);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.setDomNodeChildren"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>setDomNodeChildren (node, childNodes)](#apidoc.element.knockout.virtualElements.setDomNodeChildren)
- description and source-code
```javascript
setDomNodeChildren = function (node, childNodes) {
    if (!isStartComment(node))
        ko.utils.setDomNodeChildren(node, childNodes);
    else {
        ko.virtualElements.emptyNode(node);
        var endCommentNode = node.nextSibling; // Must be the next sibling, as we just emptied the children
        for (var i = 0, j = childNodes.length; i < j; i++)
            endCommentNode.parentNode.insertBefore(childNodes[i], endCommentNode);
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.knockout.virtualElements.virtualNodeBindingValue"></a>[function <span class="apidocSignatureSpan">knockout.virtualElements.</span>virtualNodeBindingValue (node)](#apidoc.element.knockout.virtualElements.virtualNodeBindingValue)
- description and source-code
```javascript
virtualNodeBindingValue = function (node) {
    var regexMatch = (commentNodesHaveTextProperty ? node.text : node.nodeValue).match(startCommentRegex);
    return regexMatch ? regexMatch[1] : null;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
