可以用于图片的大图预览，以及动画切换

#### 引入图片查看器组件

```jsx
//引入
import PictureViewer from 'react-photos-viewer/build'
```

### 使用

```jsx

export default function App() {
	/*
		*@params imageDate: string[]  图片数组   closeClick 关闭回调	
	*/
	const imageDate = []
	const [showBrowser, setShowBrowser] = useState(false)
 return (
    <div>
      <div className='show-btn' onClick={()=>setShowBrowser(true)}>显示照片</div>
   		{ showBrowser &&(
   			<PictureViewer ImageData={imageDate} closeClick={()=>setShowBrowser(false)}/>
   		)}

  </div>

 )
}
```



