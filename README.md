# CoReFix Data Samples

This repository contains samples from the data of CoReFix paper. 
The samples are code reduced versions of the files.
In case you want to see the full version of the files, we also included github urls. Each rule folder has a README and it contains the two url links per delta and the filename in the repo. 
File url links should take you directly to the file and also highlight the line where the rule was reported by static analyzer.
The other url is the link to the commit.
Please read the last section in the README about github urls.

We would like to avoid sharing the complete dataset yet and therefore for each rule we randomly sampled two instances from our dataset. 

# Structure of the repo for a single rule
```
├── AmbiguousConditional \
│   ├── delta_AmbiguousConditional.html # delta for the first sample \
│   ├── delta_AmbiguousConditional.html # delta for the second sample \
│   ├── README.md # contains github urls to original repos \
└── README.md 
``````

# How to view the samples?

Use this web-view https://anonymous54324.github.io/corefix_data/ to navigate the rules.

# Note about GitHub URLs

In rare cases github urls will not lead you to the correct place. This is not a bug in our code but it is related to how libgit library works. We do not store the full files in our dataset to save memory but fetch them on the fly via libgit. Those commit hashes work for file fetching process because libgit also has some internal logic to handle rebases, merge commits and other things. Therefore, the commit hashes we save are meant to be used for file fetching via libgit not for url creation. That's why, when used as urls, the commit shas might not lead to the right place.

In such cases, you can open the github repo, find the file (filename is provided in html files) and search the history of that file. Some of the commits close to the given commit hash must contain the presented changes.




# Rules

[AmbiguousConditional](./AmbiguousConditional)

[AngularSceProviderDisabled](./AngularSceProviderDisabled)

[ArithmeticOperationWithNaN](./ArithmeticOperationWithNaN)

[ArrayConstructor](./ArrayConstructor)

[ArrayMethodOnNonArray](./ArrayMethodOnNonArray)

[AssignToExports](./AssignToExports)

[AssignmentWithSameVarOnLeftAndRight](./AssignmentWithSameVarOnLeftAndRight)

[BadAwaitExpression](./BadAwaitExpression)

[BadOperandForBitwiseOperation](./BadOperandForBitwiseOperation)

[BadWrapperObjectCreation](./BadWrapperObjectCreation)

[BitwiseOperationSignChecked](./BitwiseOperationSignChecked)

[BooleanObjectCreation](./BooleanObjectCreation)

[CallbackShouldReturn](./CallbackShouldReturn)

[CodeInjection](./CodeInjection)

[CollectionArraySizeMatch](./CollectionArraySizeMatch)

[CollectionQueriedButNeverUpdated](./CollectionQueriedButNeverUpdated)

[CollectionUpdatedButNeverQueried](./CollectionUpdatedButNeverQueried)

[CommaOrSwitch](./CommaOrSwitch)

[CommandInjection](./CommandInjection)

[CompareTypeofToString](./CompareTypeofToString)

[ComparisonToNaN](./ComparisonToNaN)

[ConditionWithAssign](./ConditionWithAssign)

[ConfusedOperator](./ConfusedOperator)

[ConfusedRegex](./ConfusedRegex)

[ContentLengthInCode](./ContentLengthInCode)

[ContentTypeNoCharset](./ContentTypeNoCharset)

[ControlFlowJumpFromFinally](./ControlFlowJumpFromFinally)

[CopyPasteError](./CopyPasteError)

[DOMXSS](./DOMXSS)

[DateMonthDecember](./DateMonthDecember)

[DateMonthIndex](./DateMonthIndex)

[DeleteOfNonProperty](./DeleteOfNonProperty)

[Deserialization](./Deserialization)

[DisablePoweredBy](./DisablePoweredBy)

[DuplicateCaseSwitch](./DuplicateCaseSwitch)

[DuplicateVueProperty](./DuplicateVueProperty)

[ElectronInsecureWebPreferences](./ElectronInsecureWebPreferences)

[ElectronLoadInsecureContent](./ElectronLoadInsecureContent)

[EmberInitializerDeprecation](./EmberInitializerDeprecation)

[EqualityMisplacedParentheses](./EqualityMisplacedParentheses)

[ExceptionIsNotThrown](./ExceptionIsNotThrown)

[ExpectsObjectDislikesPrimitive](./ExpectsObjectDislikesPrimitive)

[FirefoxImageNonStandard](./FirefoxImageNonStandard)

[ForEachReturns](./ForEachReturns)

[ForbiddenUsageInStrictMode](./ForbiddenUsageInStrictMode)

[FormatString](./FormatString)

[FunctionDeclarationInBlock](./FunctionDeclarationInBlock)

[GlobalReplacementRegex](./GlobalReplacementRegex)

[HTTPSourceWithUncheckedType](./HTTPSourceWithUncheckedType)

[HardcodedNonCryptoSecret](./HardcodedNonCryptoSecret)

[HardcodedSecret](./HardcodedSecret)

[HttpToHttps](./HttpToHttps)

[ImplicitCoercionInOperator](./ImplicitCoercionInOperator)

[InOperatorBadLHS](./InOperatorBadLHS)

[IncompatibleTypesInComparison](./IncompatibleTypesInComparison)

[IncompleteRegex](./IncompleteRegex)

[IncorrectHtmlEscape](./IncorrectHtmlEscape)

[InsecureCipherNoIntegrity](./InsecureCipherNoIntegrity)

[InsecureCipher](./InsecureCipher)

[InsecureHash](./InsecureHash)

[InsecureTLSConnection](./InsecureTLSConnection)

[InsufficientValidation](./InsufficientValidation)

[IntrospectionEnabled](./IntrospectionEnabled)

[LimitGraphqlDepth](./LimitGraphqlDepth)

[LoopConditionLengthMissing](./LoopConditionLengthMissing)

[LoopDOS](./LoopDOS)

[MemberExpressionTypo](./MemberExpressionTypo)

[MissingApiCallGet](./MissingApiCallGet)

[MissingApiCallReject](./MissingApiCallReject)

[MissingCloseOnSomePath](./MissingCloseOnSomePath)

[MissingClose](./MissingClose)

[NoCryptoTimingAttacks](./NoCryptoTimingAttacks)

[NoEffectExpression](./NoEffectExpression)

[NoHardcodedCredentials](./NoHardcodedCredentials)

[NoHardcodedPasswords](./NoHardcodedPasswords)

[NoRateLimitingForExpensiveWebOperation](./NoRateLimitingForExpensiveWebOperation)

[NoRateLimitingForLogin](./NoRateLimitingForLogin)

[NoSqli](./NoSqli)

[NoZeroReturnedInSort](./NoZeroReturnedInSort)

[NodeBufferNoOffset](./NodeBufferNoOffset)

[NonLocalLoopVar](./NonLocalLoopVar)

[NonYieldingGenerator](./NonYieldingGenerator)

[NotTrimmed](./NotTrimmed)

[OR](./OR)

[ObjectConstructor](./ObjectConstructor)

[OperatorPrecedence](./OperatorPrecedence)

[OverwriteAssignment](./OverwriteAssignment)

[PT](./PT)

[PrimitiveInstanceOf](./PrimitiveInstanceOf)

[PrototypePollution](./PrototypePollution)

[PureFunctionReturnValueIgnored](./PureFunctionReturnValueIgnored)

[RHSPrimitiveType](./RHSPrimitiveType)

[ReactApiTypo](./ReactApiTypo)

[ReactArrayLengthLogicalAnd](./ReactArrayLengthLogicalAnd)

[ReactContextTypes](./ReactContextTypes)

[ReactControlledUncontrolledFormElement](./ReactControlledUncontrolledFormElement)

[ReactDeprecatedElementProp](./ReactDeprecatedElementProp)

[ReactEventHandlerThis](./ReactEventHandlerThis)

[ReactForbiddenMethodInRender](./ReactForbiddenMethodInRender)

[ReactForwardPropsToSuper](./ReactForwardPropsToSuper)

[ReactIdentifierTypo](./ReactIdentifierTypo)

[ReactInClass](./ReactInClass)

[ReactIncorrectReturnValue](./ReactIncorrectReturnValue)

[ReactInvalidEventHandlerType](./ReactInvalidEventHandlerType)

[ReactLegacyLifecycleMethod](./ReactLegacyLifecycleMethod)

[ReactMaybeMissingEventHandlerCleanup](./ReactMaybeMissingEventHandlerCleanup)

[ReactMissingArrayKeys](./ReactMissingArrayKeys)

[ReactMissingCleanup](./ReactMissingCleanup)

[ReactMissingEventHandlerCleanup](./ReactMissingEventHandlerCleanup)

[ReactModifyProps](./ReactModifyProps)

[ReactModifyState](./ReactModifyState)

[ReactReservedPropsUsed](./ReactReservedPropsUsed)

[ReactSetInnerHtml](./ReactSetInnerHtml)

[ReactShouldConstructProps](./ReactShouldConstructProps)

[ReactStateFromProps](./ReactStateFromProps)

[ReactThisInFunctionComponent](./ReactThisInFunctionComponent)

[ReactThisInStaticLifecycleMethod](./ReactThisInStaticLifecycleMethod)

[ReactTypeCreatorUsedAsType](./ReactTypeCreatorUsedAsType)

[ReactVoidHtmlElementWithChildren](./ReactVoidHtmlElementWithChildren)

[ReactWrongStyleProperty](./ReactWrongStyleProperty)

[ReactWrongStyleType](./ReactWrongStyleType)

[RegExpBadCharRange](./RegExpBadCharRange)

[RegExpStringInReplace](./RegExpStringInReplace)

[RepeatFuncArg](./RepeatFuncArg)

[ReplaceWithSameString](./ReplaceWithSameString)

[ReplacementRegex](./ReplacementRegex)

[RequireAsConstructor](./RequireAsConstructor)

[ServerLeak](./ServerLeak)

[ShiftOverflow](./ShiftOverflow)

[Sqli](./Sqli)

[Ssrf](./Ssrf)

[Ssti](./Ssti)

[StringMethodOnNonString](./StringMethodOnNonString)

[SuperDuplicated](./SuperDuplicated)

[ThisBeforeSuper](./ThisBeforeSuper)

[TooPermissiveCorsHeader](./TooPermissiveCorsHeader)

[TooPermissiveCorsPostMessage](./TooPermissiveCorsPostMessage)

[TooSmallRsaKeySizeUsed](./TooSmallRsaKeySizeUsed)

[TypeofNotComparedToAnything](./TypeofNotComparedToAnything)

[UnusedIterator](./UnusedIterator)

[UnusedLoopVar](./UnusedLoopVar)

[UpdateApi](./UpdateApi)

[UsageOfUninitializedVariable](./UsageOfUninitializedVariable)

[UseArrowFunction](./UseArrowFunction)

[UseCsurfForExpress](./UseCsurfForExpress)

[UseGetFullYear](./UseGetFullYear)

[UseHelmetForExpress](./UseHelmetForExpress)

[UseIsArrayToCheckForArrays](./UseIsArrayToCheckForArrays)

[UseLowercaseTagsForXHTML](./UseLowercaseTagsForXHTML)

[UseSecureWebsockets](./UseSecureWebsockets)

[UseStrictWrong](./UseStrictWrong)

[Utf8Literal](./Utf8Literal)

[VarDeclConflict](./VarDeclConflict)

[VueIncorrectMethodsPropertyType](./VueIncorrectMethodsPropertyType)

[VueInvalidComponentName](./VueInvalidComponentName)

[VueMissingCleanup](./VueMissingCleanup)

[VueMountOnHtmlElement](./VueMountOnHtmlElement)

[VuePropertyUpdateOnVueInstance](./VuePropertyUpdateOnVueInstance)

[VuePropsDeclAssignment](./VuePropsDeclAssignment)

[VuePropsInsideTypos](./VuePropsInsideTypos)

[VueReservedProperty](./VueReservedProperty)

[VueThisInComponentPropertyArrowFunction](./VueThisInComponentPropertyArrowFunction)

[WebCookieHttpOnlyDisabledByDefault](./WebCookieHttpOnlyDisabledByDefault)

[WebCookieHttpOnlyDisabledExplicitly](./WebCookieHttpOnlyDisabledExplicitly)

[WebCookieSecureDisabledByDefault](./WebCookieSecureDisabledByDefault)

[WebCookieSecureDisabledExplicitly](./WebCookieSecureDisabledExplicitly)

[WrongCleanupUsed](./WrongCleanupUsed)

[WrongComparisonOperatorInSort](./WrongComparisonOperatorInSort)

[WrongTypeComparison](./WrongTypeComparison)

[XSS](./XSS)

[reDOS](./reDOS)

