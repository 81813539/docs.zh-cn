---
title: "迁移和互操作性 | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-wpf"
ms.tgt_pltfrm: ""
ms.topic: "article"
f1_keywords: 
  - "AutoGeneratedOrientationPage"
helpviewer_keywords: 
  - "控件 [WPF 互操作性]"
  - "互操作性 [WPF]"
  - "迁移 [WPF]"
  - "Windows 窗体控件 [WPF 互操作性]"
  - "Windows Presentation Foundation, 互操作性"
  - "Windows Presentation Foundation, 迁移"
  - "WPF, 互操作性"
  - "WPF, 迁移"
ms.assetid: d655de05-bf63-4814-bc64-6b3be01c70a2
caps.latest.revision: 41
author: "dotnet-bot"
ms.author: "dotnetcontent"
manager: "wpickett"
caps.handback.revision: 41
---
# 迁移和互操作性
本页包含一些指向文档的链接，这些文档讨论如何在 [!INCLUDE[TLA#tla_winclient](../../../../includes/tlasharptla-winclient-md.md)] 应用程序和其他类型的 [!INCLUDE[TLA#tla_win](../../../../includes/tlasharptla-win-md.md)] 应用程序之间实现互操作。  
  
## 本节内容  
 [WPF 和 Windows 窗体互操作](../../../../docs/framework/wpf/advanced/wpf-and-windows-forms-interoperation.md)  
 [WPF 和 Win32 互操作](../../../../docs/framework/wpf/advanced/wpf-and-win32-interoperation.md)  
 [WPF 和 Direct3D9 互操作](../../../../docs/framework/wpf/advanced/wpf-and-direct3d9-interoperation.md)  
  
## 参考  
  
|术语|定义|  
|--------|--------|  
|<xref:System.Windows.Forms.Integration.WindowsFormsHost>|可用于将 [!INCLUDE[TLA#tla_winforms](../../../../includes/tlasharptla-winforms-md.md)]控件作为 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 页的元素来承载的元素。|  
|<xref:System.Windows.Forms.Integration.ElementHost>|可用于承载 [!INCLUDE[TLA#tla_winclient](../../../../includes/tlasharptla-winclient-md.md)] 控件的 [!INCLUDE[TLA#tla_winforms](../../../../includes/tlasharptla-winforms-md.md)]控件。|  
|<xref:System.Windows.Interop.HwndSource>|在 [!INCLUDE[TLA2#tla_win32](../../../../includes/tla2sharptla-win32-md.md)] 应用程序中承载 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 区域。|  
|<xref:System.Windows.Interop.HwndHost>|用来定义一些基本功能的 <xref:System.Windows.Forms.Integration.WindowsFormsHost> 的基类，在由 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 应用程序承载时，基于 HWND 的所有技术都将使用这些功能。  将该类归为子类可以将 [!INCLUDE[TLA2#tla_win32](../../../../includes/tla2sharptla-win32-md.md)] 窗口承载到 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 应用程序中。|  
|<xref:System.Windows.Interop.BrowserInteropHelper>|一种帮助器类，用来为浏览器所承载的 [!INCLUDE[TLA2#tla_winclient](../../../../includes/tla2sharptla-winclient-md.md)] 应用程序报告浏览器环境条件。|  
  
## 相关章节