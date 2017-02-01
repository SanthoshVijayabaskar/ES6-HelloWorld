## Modal HTML

```html
<div class="modal fade">
		<div class="modal-dialog">
			<div class="modal-content" style="height:375px;width:450px;margin-left: 100px;">
				<div class="modal-header" style="border-bottom: none;">	
					<b style="font-size:15px">Plans And Products</b>
				</div>
				<div class="modal-body" >
				<table>
					<tr>
						<td style="width: 170px;">
							Available Plans
							<select size="5" multiple ng-model="Toselect" ng-options="item for item in nonSelectedOptions" style="width: 170px;height:150px;"></select>         
						</td>
						<td style="padding :10px">
					    	<input id="moveright" type="button" value=">" style="width: 30px;" ng-click="moveItem(Toselect, nonSelectedOptions,selectedOptions).bind(this)" />
					    	<br>
					    	<input id="moverightall" type="button" value=">>" style="width: 30px;margin-top: 5px;" ng-click="moveAll(nonSelectedOptions,selectedOptions).bind(this)" />
					    	<br>
					    	<input id="move left" type="button" value="<" style="width: 30px;margin-top: 5px;" ng-click="moveItem(toUnSelect, selectedOptions,nonSelectedOptions).bind(this)" />    
					    	<br>
					    	<input id="moveleftall" type="button" value="<<" style="width: 30px;margin-top: 5px;" ng-click="moveAll(selectedOptions,nonSelectedOptions).bind(this)" />
						</td>
					    <td style="width: 170px;">   
					    	Selected Plans                                           
		   					<select size="5" multiple ng-model="toUnSelect" ng-options="item for item in selectedOptions" style="width: 170px;height:150px;"></select>
		    			</td>
	    			</tr>
				</table>
				   
				</div>
				
				<div class="modal-footer" style="border-top: none;">
					
					    <button type="button" data-dismiss="modal" aria-hidden="true" class="btn btn-primary btn-lg" style="padding: 6px 15px 6px 15px;font-size: 14px;">Done</button> 
					    
					 <!--   <button type="button" class="btn btn-default btn-lg" data-dismiss="modal" aria-hidden="true" style="padding: 6px 12px 6px 12px;font-size: 14px;">No</button>
					 -->
				</div>
				
			</div>
		</div>
</div>
				

```
