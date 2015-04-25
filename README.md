# NSDictionary-SafeAccess
非常有助于IOS字典读写的轻量级扩展,Very useful safe accessors for NSDictionary,a lightweight NSDictionary access category
#妈妈再也不用担心NULL啦

#使用方法 
##读取 getter
	NSDictionary *responseObject = /.......
	
	NSDictionary *dic = [responseObject dictionaryForKey:@"object"];
	
	NSArray *array = [responseObject arrayForKey:@"array"];
	
	NSString *string = [responseObject stringForKey:@"string"];
	
	long long date = [responseObject longLongForKey:@"date"];
	
	NSNumber *number = [responseObject numberForKey:@"number"];
	
	NSInteger count = [responseObject integerForKey:@"count"];
	
	BOOL b = [responseObject boolForKey:@"count"]; 
	
	CGPoint point = [responseObject pointForKey:@"point"]; 
	
	CGFloat f = [responseObject CGFloatForKey:@"float"]; 
	
	CGRect rect = [responseObject rectForKey:@"rect"]; 
	
	CGSize size = [responseObject sizeForKey:@"size"]; 
##写入 setter
	NSMutableDictionary *dict = [NSMutableDictionary dictionary];
	
    [dict setObj:@"334" forKey:@"obj"];
    
    [dict setString:@"string" forKey:@"str"];
    
    [dict setBool:YES forKey:@"b"];
    
    [dict setInt:1 forKey:@"intvalue"];
    
    [dict setCGFloat:1.1 forKey:@"float"];
    
    [dict setPoint:CGPointMake(1, 1) forKey:@"point"];
    
    [dict setSize:CGSizeMake(111, 111) forKey:@"size"];
    
    [dict setRect:CGRectMake(0, 0, 0, 0) forKey:@"rect"];
