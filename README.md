# CodeHighLightTemp

```as3
trace('hello world');
```
```as3
public class CompensateGetInfoService extends HttpService
{
	[Inject]
	public var compensateProxy:CompensateProxy;
	
	public function CompensateGetInfoService()
	{
		super(AppServiceNameConst.COMPENSATE_GET_INFO);
	}
	
	override public function success(value:Object):void
	{
		compensateProxy.analysisPlayerInfo(value);
		applyCallback(null);
	}
}
```
```as3
public class FrameworkBundle implements IBundle
{
	/**
	 * Constructor
	 **/
	public function FrameworkBundle()
	{
	}
	
	public function extend(context:IContext):void
	{
		context.install( 
			AssetsExtension, 
			PopupExtension,
			HttpExtension,
			FacebookExtension,
			DebugConsoleExtension
		);
		
		context.configure( 
			FacebookConfig
		);
	}
}
```
```as3
serversFactory.getEmptyService(AppServiceNameConst.ACTIVITY_PRODUCT_GET_REWARD).send([AppData.myId,activityId,rewardIndex,TimeManager.getTime()]);
```
```as3
eventDispatcher.dispatchEvent(new CommonEvent(CommonEvent.ACH_POINT_UPDATE));
```
```as3
addViewListener(ActivityBaseEvent.CALL_ACTIVITY_STORY,callActivityStortyHandler);
```
```as3
addContextListener(CommonEvent.ACH_COMPLETE_SHOW, showHandler);
```
```as3
dispatchEvent(new MasteryUpgradeViewEvent(MasteryUpgradeViewEvent.CLICK_SHARE,_data));
```
```xml
<widget folder="">
    <item id="CommonView"		p = "1">/assets/widget/common.swf</item>
    <item id="TipsView"			p = "1">/assets/widget/tips.swf</item>
    <item id="MessagePanelView"	p = "1">/assets/widget/common.swf</item>
</widget>
```
```as3
_view = _assetsFactory.getMovieClip('petShopView', AppAssetsConst.PET_SHOP_VIEW);
this.addChild(_view);
```
```as3
skin = _assetsFactory.getMovieClip('goodsItem',AppAssetsConst.QUICK_BUY_VIEW);
_sprite.addChild(skin);
```
```as3
app.engine.widget // UI框架

```
```as3
context.injector.map(IHttpServiceFactory).toSingleton(HttpServiceFactory); // 映射接口到类型，并且是单例
inject.map(JsProxy).toValue(jsProxy); // 映射实例
context.injector.map(IDirectCommandMap).toType(DirectCommandMap); // 映射类型
```
```as3
```
```as3
```
```as3
```
```as3
```
```as3
```