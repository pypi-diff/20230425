# Comparing `tmp/mplot-0.220004.tar.gz` & `tmp/mplot-0.220005.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mplot-0.220004.tar", last modified: Fri Feb 25 05:14:47 2022, max compression
+gzip compressed data, was "mplot-0.220005.tar", last modified: Mon Apr 24 22:20:50 2023, max compression
```

## Comparing `mplot-0.220004.tar` & `mplot-0.220005.tar`

### file list

```diff
@@ -1,16 +1,15 @@
-drwxrwxrwx   0        0        0        0 2022-02-25 05:14:47.000000 mplot-0.220004/
--rw-rw-rw-   0        0        0      261 2022-02-25 05:14:47.000000 mplot-0.220004/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-02-25 05:14:47.000000 mplot-0.220004/mplot/
--rw-rw-rw-   0        0        0        0 2021-02-04 23:08:00.000000 mplot-0.220004/mplot/__init__.py
--rw-rw-rw-   0        0        0    11345 2021-02-04 23:09:06.000000 mplot-0.220004/mplot/color.py
--rw-rw-rw-   0        0        0     1772 2021-02-04 23:09:06.000000 mplot-0.220004/mplot/createdate.py
--rw-rw-rw-   0        0        0      767 2022-02-25 04:00:41.000000 mplot-0.220004/mplot/example_of_mplot.py
--rw-rw-rw-   0        0        0    87697 2022-02-25 05:12:35.000000 mplot-0.220004/mplot/plot.py
-drwxrwxrwx   0        0        0        0 2022-02-25 05:14:47.000000 mplot-0.220004/mplot.egg-info/
--rw-rw-rw-   0        0        0      261 2022-02-25 05:14:47.000000 mplot-0.220004/mplot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2022-02-25 05:14:47.000000 mplot-0.220004/mplot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-02-25 05:14:47.000000 mplot-0.220004/mplot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2021-02-04 23:09:06.000000 mplot-0.220004/mplot.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        6 2022-02-25 05:14:47.000000 mplot-0.220004/mplot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-02-25 05:14:47.000000 mplot-0.220004/setup.cfg
--rw-rw-rw-   0        0        0      309 2022-02-25 05:13:00.000000 mplot-0.220004/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-24 22:20:50.698930 mplot-0.220005/
+-rw-rw-rw-   0        0        0      261 2023-04-24 22:20:50.697933 mplot-0.220005/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-24 22:20:50.693940 mplot-0.220005/mplot/
+-rw-rw-rw-   0        0        0    11345 2022-02-25 05:22:23.000000 mplot-0.220005/mplot/color.py
+-rw-rw-rw-   0        0        0     1772 2022-02-25 05:22:25.000000 mplot-0.220005/mplot/createdate.py
+-rw-rw-rw-   0        0        0      900 2023-04-24 22:11:08.000000 mplot-0.220005/mplot/example_of_mplot.py
+-rw-rw-rw-   0        0        0    87959 2023-04-24 22:15:02.000000 mplot-0.220005/mplot/plot.py
+drwxrwxrwx   0        0        0        0 2023-04-24 22:20:50.697933 mplot-0.220005/mplot.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-04-24 22:20:50.000000 mplot-0.220005/mplot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-04-24 22:20:50.000000 mplot-0.220005/mplot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-24 22:20:50.000000 mplot-0.220005/mplot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-24 22:20:50.000000 mplot-0.220005/mplot.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        6 2023-04-24 22:20:50.000000 mplot-0.220005/mplot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-24 22:20:50.698930 mplot-0.220005/setup.cfg
+-rw-rw-rw-   0        0        0      309 2023-04-24 21:17:43.000000 mplot-0.220005/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `mplot-0.220004/mplot/color.py` & `mplot-0.220005/mplot/color.py`

 * *Files identical despite different names*

### Comparing `mplot-0.220004/mplot/createdate.py` & `mplot-0.220005/mplot/createdate.py`

 * *Files identical despite different names*

### Comparing `mplot-0.220004/mplot/plot.py` & `mplot-0.220005/mplot/plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -977,15 +977,14 @@
         i = pair[1]
         newhandles.append(handles[i])
         newlabels.append(labels[i])
     return newhandles,newlabels
 
 
 
-
 def sortlegends(handles,labels,legendorder,ncols,legenddirection):
     if type(legendorder) == type('string'):
         newhandles,newlabels = sortlegends_string(handles,labels,legendorder.upper())
     elif type(legendorder) in [type([0,1]),type((0,1))]:
         newhandles,newlabels = sortlengend_order(handles,labels,legendorder)
     else:
         raise Exception()
@@ -1027,15 +1026,15 @@
         self.second_y_axis = axy2
 class figsubcls():
     def __init__(self,fig,axs):
         self.fig = fig
         self.axs = axs
 
 
-def savesubplot(objects,fig,axs,fname,rawext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save):
+def savesubplot(objects,fig,axs,fname,rawext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save,legendtitle = None):
     rawext = rawext.replace('.','')
     ext = rawext
     fig.tight_layout()
     if ext == 'pdf2ps':
         ext = 'pdf'   
     if makelegend(objects,None):
         handles = []
@@ -1043,15 +1042,15 @@
         for axrow in axs:
             for ax in axrow:
                 hndls, lbls = ax.get_legend_handles_labels()    
                 handles += hndls
                 labels += lbls
             
         handles,labels = sortlegends(handles,labels,legendorder,ncols,legenddirection.upper())
-        lgd = fig.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc)
+        lgd = fig.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc,title = legendtitle)
         if not save:
             matplotlib.pyplot.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc)
             fig.tight_layout()
             return figcls(fig,axs)
         pyplot.savefig(fname+'.'+ext,bbox_extra_artists=(lgd,), bbox_inches='tight',dpi = resolution)
     elif not save:
         return figcls(fig,ax1,axx2,axy2)
@@ -1062,15 +1061,15 @@
     if rawext == 'pdf2ps':
         os.system('pdf2ps '+fname+'.pdf '+fname+'.ps')
     return None
 
 
 
 
-def saveplot(objects,fig,ax1,axy2,axx2,fname,rawext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save,legend = None):
+def saveplot(objects,fig,ax1,axy2,axx2,fname,rawext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save,legend = None,legendtitle = None):
     rawext = rawext.replace('.','')
     ext = rawext    
     if ext == 'pdf2ps':
         ext = 'pdf'
     ax1.set_xlim(minmax['x'][0],minmax['x'][1])
     ax1.set_ylim(minmax['y'][0],minmax['y'][1])
     if axy2 is not None:
@@ -1086,17 +1085,17 @@
         if axx2 is not None:
             htemp, ltemp = axx2.get_legend_handles_labels()
             handles+= htemp
             labels += ltemp
         if legend != None:
             labels = legend
         handles,labels = sortlegends(handles,labels,legendorder,ncols,legenddirection.upper())
-        lgd = ax1.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc)
+        lgd = ax1.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc,title = legendtitle)
         if not save:
-            matplotlib.pyplot.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc)
+            matplotlib.pyplot.legend(handles,labels,ncol=ncols,loc = lpos,bbox_to_anchor=lloc,title = legendtitle)
             fig.tight_layout()
             return figcls(fig,ax1,axx2,axy2)
         pyplot.savefig(fname+'.'+ext,bbox_extra_artists=(lgd,), bbox_inches='tight',dpi = resolution)
     elif not save:
         fig.tight_layout()
         return figcls(fig,ax1,axx2,axy2)
     else:
@@ -2420,29 +2419,29 @@
             if doalphas:
                 obj.alphas.append(1)
     
             
     
 
 
-def makepiecharts(objects,rawfname,write,fontsize,rawfigsize,frame,ext,lloc,lpos,ncols,resolution,colorlist,title,legendorder,legenddirection,save):
+def makepiecharts(objects,rawfname,write,fontsize,rawfigsize,frame,ext,lloc,lpos,ncols,resolution,colorlist,title,legendorder,legenddirection,save,legendtitle):
     newobjects = []
     ave = (rawfigsize[0]+rawfigsize[1])/2.0
     figsize = (ave,ave)
     for i in range(0,len(objects)):
         obj = objects[i]
         if obj.name != 'pie':
             newobjects.append(obj)
             continue
         fname = makepiename(objects,rawfname,i)
         addpiecolor(colorlist,obj)
         fig,ax1,axy2,axx2 = initplot([obj],fontsize,figsize,frame,False,False)
         maketitle(title)
         legend = makepie(obj,ax1)
-        saveplot(objects,fig,ax1,axy2,axx2,fname,ext,lloc,lpos,ncols,legendorder,legenddirection,resolution,save,legend = legend)
+        saveplot(objects,fig,ax1,axy2,axx2,fname,ext,lloc,lpos,ncols,legendorder,legenddirection,resolution,save,legend = legend,legendtitle = legendtitle)
     return newobjects
 
 def getval(string):
     if '/' in string:
         return createdate.convertdatetime(string)
     if string.count('-') > 1:
         return createdate.convertdatetime(string)
@@ -2517,22 +2516,22 @@
         r += 1
     return objects,(r,maxc)
 
 def displaysubplots(rawobjects,fname,write = False,fontsize = FONTSIZE,figsize = (8,6),frame = True,ext = 'png',lloc = (0.5,0),lpos = 'upper center',subtitles = None,
             ncols = 3,gridlines=False,xgridlines = False,ygridlines = False,gridlinestyle = {'style' :'--','color': BLACK,'subticks' : False,'alpha' : 0.3},resolution = 300,colorlist = COLORLIST,title = None,
             xlabel = None,xticks = None,xsubticks = 0,xrotation = 0,xalign = 'center',xminmax = None,xzero = False,xfontsize = FONTSIZE,xaxisdisplay = True,xlabels = [],
             ylabel = None,yticks = None,ysubticks = 0,yrotation = 0,yalign = 'right',yminmax = None,yzero = False, yfontsize = FONTSIZE,yaxisdisplay = True,ylabels = [],
-            axisfontsize = None,areastacked = True,chartstacked = False,stacked = None,legendorder = 'normal',legenddirection = 'horizontal',lowmemory=False,
+            axisfontsize = None,areastacked = True,chartstacked = False,stacked = None,legendorder = 'normal',legenddirection = 'horizontal',legendtitle = None,lowmemory=False,
             xlog=False,xlogbase=10,xlog0 = None,ylog=False,ylogbase=10,ylog0 = None,save = True,dynamic = False):
     if lowmemory == True:
         objects = rawobjects
     else:
         objects = copy.deepcopy(rawobjects)
     objects,subplotdim = setsubplotposition(objects)
-    objects = makepiecharts(objects,fname,write,fontsize,figsize,frame,ext,lloc,lpos,ncols,resolution,colorlist,title,legendorder,legenddirection,save)
+    objects = makepiecharts(objects,fname,write,fontsize,figsize,frame,ext,lloc,lpos,ncols,resolution,colorlist,title,legendorder,legenddirection,save,legendtitle)
     if objects == []:
         return
     writeout(objects,fname,write)        
     objects = fixcolor(objects,colorlist)    
     objects = fixhistogramfit(objects)
     objects = fixareas(objects,areastacked,stacked)
     objects,cats,stackcharts,stackhcharts,width,mindiff,offsets = handlechartboxplotoverlap(objects,chartstacked,stacked)
@@ -2556,27 +2555,27 @@
     objects = fixscale(objects,trans)
     for obj in objects:
         obj.func(obj,axs[obj.subplotposition[0],obj.subplotposition[1]])
     makesubtitle(fig,axs,title,subtitles,subplotdim)
     for axrow in axs:
         for ax in axrow:
             ax.label_outer()
-    img = savesubplot(objects,fig,axs,fname,ext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save)
+    img = savesubplot(objects,fig,axs,fname,ext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save,legendtitle = legendtitle)
     return img
     
 
 def display(rawobjects,fname,write = False,fontsize = FONTSIZE,figsize = (8,6),frame = True,ext = 'png',lloc = (0.5,-0.1),lpos = 'upper center',
             ncols = 3,gridlines=False,xgridlines = False,ygridlines = False,gridlinestyle = {'style' :'--','color': BLACK,'subticks' : False,'alpha' : 0.3},resolution = 300,colorlist = COLORLIST,title = None,
             xlabel = None,xticks = None,xsubticks = 0,xrotation = 0,xalign = 'center',xminmax = None,xzero = False,xfontsize = FONTSIZE,xaxisdisplay = True,
             ylabel = None,yticks = None,ysubticks = 0,yrotation = 0,yalign = 'right',yminmax = None,yzero = False, yfontsize = FONTSIZE,yaxisdisplay = True,
             second_ylabel = SECOND_YLABEL,second_yticks = SECOND_YTICKS,second_ysubticks = SECOND_YSUBTICKS,second_yrotation = SECOND_YROTATION,
             second_yalign = SECOND_YALIGN,second_yminmax = SECOND_YMINMAX,second_yzero = SECOND_YZERO,second_yfontsize = SECOND_YFONTSIZE,second_yaxisdisplay = True,
             second_xlabel = SECOND_XLABEL,second_xticks = SECOND_XTICKS,second_xsubticks = SECOND_XSUBTICKS,second_xrotation = SECOND_XROTATION,
             second_xalign = SECOND_XALIGN,second_xminmax = SECOND_XMINMAX,second_xzero = SECOND_XZERO,second_xfontsize = SECOND_XFONTSIZE,second_xaxisdisplay = True,
-            axisfontsize = None,areastacked = True,chartstacked = False,stacked = None,legendorder = 'normal',legenddirection = 'horizontal',lowmemory=False,
+            axisfontsize = None,areastacked = True,chartstacked = False,stacked = None,legendorder = 'normal',legenddirection = 'horizontal',legendtitle = None,lowmemory=False,
             xlog=False,xlogbase=10,xlog0 = None,ylog=False,ylogbase=10,ylog0 = None,second_ylog=False,second_ybase=10,second_ylog0 = None,second_xlog=False,
             second_xbase=10,second_xlog0 = None,save = True,dynamic = False):
 
     '''
     ext is one of: 'png' 'eps' 'pdf' 'pdf2ps'
     legendorder is either: 'reverse' 'normal' 'alphabetic' (reverse, reverses the order, normal does nothing, alphabetic orders alphabetically)
     or : legendorder is a list e.g. ['leg 1','leg 2'...] of the desired order
@@ -2584,15 +2583,15 @@
     dynamic is needed if want to use tkinter and have the x and y values display.
     there is a gremlin in that setting x or y labels interferes with the dynamic nature.
     '''
     if lowmemory == True:
         objects = rawobjects
     else:
         objects = copy.deepcopy(rawobjects)
-    objects = makepiecharts(objects,fname,write,fontsize,figsize,frame,ext,lloc,lpos,ncols,resolution,colorlist,title,legendorder,legenddirection,save)
+    objects = makepiecharts(objects,fname,write,fontsize,figsize,frame,ext,lloc,lpos,ncols,resolution,colorlist,title,legendorder,legenddirection,save,legendtitle = legendtitle)
     if objects == []:
         return
     writeout(objects,fname,write)        
     objects = fixcolor(objects,colorlist)    
     objects = fixhistogramfit(objects)
     objects = fixareas(objects,areastacked,stacked)
     objects,cats,stackcharts,stackhcharts,width,mindiff,offsets = handlechartboxplotoverlap(objects,chartstacked,stacked)
@@ -2626,13 +2625,13 @@
             obj.func(obj,axy2)
         elif obj.secondxaxis:
             obj.func(obj,axx2)
         else:
             obj.func(obj,ax1)
     maketitle(title)
     hideaxes(ax1,axy2,axx2,xaxisdisplay,yaxisdisplay,second_yaxisdisplay,second_xaxisdisplay)
-    img = saveplot(objects,fig,ax1,axy2,axx2,fname,ext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save)
+    img = saveplot(objects,fig,ax1,axy2,axx2,fname,ext,lloc,lpos,ncols,legendorder,legenddirection,minmax,resolution,save,legendtitle = legendtitle)
     return img
 
 
 ## add a category version of lines.
```

