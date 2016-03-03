# XAMLColorOverride

A sample made to demonstrate XAML style overrides

```xml
<?xml version="1.0" encoding="UTF-8"?>
<ContentPage xmlns="http://xamarin.com/schemas/2014/forms" xmlns:x="http://schemas.microsoft.com/winfx/2009/xaml" x:Class="XAMLColorOverride.TestPage">
	<ContentPage.Resources>
        <ResourceDictionary>
			<Style x:Key="mSubTitleStyle" TargetType="Label">
				<Setter Property="FontSize" Value="Large" />
				<Setter Property="TextColor" Value="Red" />
			</Style>
		</ResourceDictionary>
    </ContentPage.Resources>
	<ContentPage.Content>
		<StackLayout Padding="20,20,20,20">
			<Label Text="Style Only (Red + Large font)" Style="{StaticResource mSubTitleStyle}"/>
			<Label Text="Style + Overrided Color(Blue)" Style="{StaticResource mSubTitleStyle}" TextColor="Blue"/>
			<Label Text="Style + Overrided Size(Small)" Style="{StaticResource mSubTitleStyle}" FontSize="Small"/>
			<Label Text="Style + Overrided Size(Micro)" Style="{StaticResource mSubTitleStyle}" FontSize="Micro"/>
		</StackLayout>
	</ContentPage.Content>
</ContentPage>
```


![image](https://cloud.githubusercontent.com/assets/8008527/13505932/822d80ae-e149-11e5-91f3-3b234677ab0c.png)


Learn more about Styles here - Xamarin Doc here - https://developer.xamarin.com/guides/xamarin-forms/user-interface/styles/explicit/#Creating_an_Explicit_Style_in_XAML
