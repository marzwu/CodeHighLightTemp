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